# dns server

```
docker run -d --name coredns --restart=always --volume=/home/steve/gdev/stevesloka/dnsserver/:/root/ -p 53:53/udp coredns/coredns -conf /root/Corefile
```