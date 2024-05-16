First establish a VPN connection to the server, then
```bash
ssh -X username@server.domain
screen -S <session_name>
echo $STY
```
Now you're logged and can do whatever you want
To detach the screen 
<c-a>
To exit 
<c-d>
Notice that this won't kill the session, in fact
```bash
screen -list
```
will still list the previous <session_name> running in the background.
You can resume it via
```bash
screen -r <session_name>
```
and then, from within the session you can terminate it via
```bash
exit
```
If instead you want to kill one session while keeping others running, then
```bash
screen -X -S <session_name> kill
```
