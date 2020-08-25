# eingsoft_v2fly_tunnel
## portal start
```sh
docker run --name v2fly --restart always -d -v $PWD/portal.json:/etc/v2ray/config.json -p 4443:4443 v2fly/v2fly-core
```
## bridge start
```sh
v2ray --config bridge.json
```
## local use
v2ray --config local.json
