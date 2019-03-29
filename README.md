# speedInspectorRPI
> A docker image running speedtest every 10 minutes.


Intended Use: Run in a raspberry pi connected via ethernet to your main router

Log the connection speed to docker logs and run in in a raspberry pi or your main machine.

### Build docker image

```bash
docker build -t speedtest .
```

### Run docker container

```bash
docker run -d --name=speedInspector --rm speedtest
```

### Check previous recorded speeds:

```bash
docker logs speedInspector

Ping: 29.826 ms
Download: 18.15 Mbit/s
Upload: 5.21 Mbit/s
Ping: 20.798 ms
Download: 18.14 Mbit/s
Upload: 4.83 Mbit/s
Ping: 20.489 ms
Download: 19.20 Mbit/s
Upload: 4.75 Mbit/s
Ping: 38.398 ms
Download: 19.46 Mbit/s
Upload: 4.40 Mbit/s
Ping: 28.94 ms
Download: 10.01 Mbit/s
Upload: 5.06 Mbit/s
Ping: 31.304 ms
Download: 19.83 Mbit/s
Upload: 4.90 Mbit/s
Ping: 19.648 ms
Download: 17.38 Mbit/s
Upload: 5.14 Mbit/s
Ping: 20.523 ms
Download: 19.15 Mbit/s
Upload: 5.17 Mbit/s
Ping: 20.937 ms
Download: 19.36 Mbit/s
Upload: 5.07 Mbit/s
Ping: 20.604 ms
Download: 12.80 Mbit/s
Upload: 5.27 Mbit/s
Ping: 19.774 ms
Download: 18.87 Mbit/s
Upload: 4.14 Mbit/s
```

