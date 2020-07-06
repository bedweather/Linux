***#: root用户***  
***$: root用户***  
- ## 查看IP
```
# ip a
```  

```bash
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: 'ens192': <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP group default qlen 1000  

    link/ether 00:50:56:a6:98:3c brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.162/24 brd 192.168.1.255 scope global noprefixroute ens192
       valid_lft forever preferred_lft forever
    inet6 fe80::91db:a008:eaee:c9f5/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
3: br0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN group default qlen 1000
    link/ether 86:58:7a:fc:7e:83 brd ff:ff:ff:ff:ff:ff
4: virbr0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN group default qlen 1000
    link/ether 52:54:00:4f:14:a1 brd ff:ff:ff:ff:ff:ff
    inet 192.168.122.1/24 brd 192.168.122.255 scope global virbr0
       valid_lft forever preferred_lft forever
5: virbr0-nic: <BROADCAST,MULTICAST> mtu 1500 qdisc pfifo_fast master virbr0 state DOWN group default qlen 1000
    link/ether 52:54:00:4f:14:a1 brd ff:ff:ff:ff:ff:ff
6: vboxnet0: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN group default qlen 1000
    link/ether 0a:00:27:00:00:00 brd ff:ff:ff:ff:ff:ff
```

option  
-a, -all : executes specified command over all objects, it depends if command supports this option.

- ## 增加删除网卡
```
# ip a add 192.168.80.174 dev eth0
# ip a del 192.168.80.174 dev eth0
```  

