
Home
```
ip address add 192.168.0.100/24 dev eth0
ip link set eth0 up
ip route add default via 192.168.0.1 dev eth0
ip address show eth0
ping 1.1.1.1
```


Office
```
ip address add 192.168.144.235/24 dev eth0
ip link set eth0 up
ip route add default via 192.168.144.1 dev eth0
ip address show eth0

udhcpc -i eth0

ping 1.1.1.1
```



