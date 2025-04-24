# Troubleshooting

## CPU overloading: syslog
1. Get the name of the process that is using a lot of CPU
```bash
sudo tail /var/log/syslog
```
2. Kill it
```bash
killall <name_of_the_process>
```
3. Clear the log file
```bash
sudo truncate -s 0 /var/log/syslog
```

## Black screen after reboot (Arch)
You need to revert some of the changes prior to the reboot (presumably a theme of the display manager in KDE Plasma 6)
1. Login to a `tty` by pressing `Ctrl + Alt + F2` or `Ctrl + Alt + F6`

2. Set `Breeze` as the system theme
```bash
echo -e “[Theme]\nCurrent=breeze” | sudo tee /etc/sddm.conf.d/theme.conf
```

3. Restart `sddm`
```bash
sudo systemctl restart sddm
```

4. Reboot if necessary
```bash
reboot
```
