# PC status 
- List all services running in the pc.
```
$sudo service --status-all
```
- Start/stop a service
```
$sudo systemctl [start/stop][service_Name]
```
- List all the ports of the computer, then make a group of the ones that are LISTENING to something.
```
sudo lsof -i -P -n | grep LISTEN
```
