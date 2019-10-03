# dns server

```
docker run -d --name coredns --restart=always --volume=/home/steve/gdev/stevesloka/dnsserver/:/root/ -p 53:53/udp coredns/coredns -conf /root/Corefile
```

## Create static interface on OSX

```bash
$ sudo ifconfig vlan169 create
$ sudo ifconfig vlan169 inet 10.52.131.230 netmask 255.255.255.255  
```

Find port 53 in use:

```bash
sudo lsof -i :53 
```