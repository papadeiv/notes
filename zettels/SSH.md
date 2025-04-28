# SSH

## Connection to UoA servers
1. First establish a VPN connection

2. Connect to the server via `ssh`
```bash
ssh your_upi@aitken.math.auckland.ac.nz
```
3. Look which of the computational servers is less busy and connect into that
```bash
ssh your_upi@forder.math.auckland.ac.nz
```
4. To execute Julia scripts have a look at the __Installation on a server__ paragraph in [Julia](Julia.md)

5. To run a `screen` session:
```bash
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

6. To disconnect from the server run
```bash
exit
```
