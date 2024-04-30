# Update and install curl

```bash
docker run -it --name exercise ubuntu
docker exec -it exercise bash
apt-get update
apt-get -y install curl
```

### run again as curl was installed

```bash
docker run -it --name exercise ubuntu sh -c 'while true; do echo "Input website:"; read website; echo "Searching..."; sleep 1; curl http://$website; done'
>> Input website:
helsinki.fi
Searching...
<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.22.1</center>
</body>
</html>

```
