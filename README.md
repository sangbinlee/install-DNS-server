# install-DNS-server
install-DNS-server





    
    apt update -y && apt upgrade -y
    apt install bind9 bind9utils bind9-doc -y
    systemctl status bind9
    
    
    


    
    root@sodi9:/home/sangbinlee9# systemctl status bind9
    ● named.service - BIND Domain Name Server
         Loaded: loaded (/lib/systemd/system/named.service; enabled; vendor preset: enabled)
         Active: active (running) since Fri 2023-11-24 15:51:14 KST; 1min 12s ago
           Docs: man:named(8)
       Main PID: 801 (named)
          Tasks: 10 (limit: 18901)
         Memory: 13.2M
            CPU: 77ms
         CGroup: /system.slice/named.service
                 └─801 /usr/sbin/named -u bind
    
    Nov 24 15:51:15 sodi9.store named[801]: listening on IPv4 interface br-d7c58f5a5c3c, 172.22.0.1#53
    Nov 24 15:51:15 sodi9.store named[801]: listening on IPv4 interface br-0bc2a079b319, 172.20.0.1#53
    Nov 24 15:51:15 sodi9.store named[801]: listening on IPv4 interface br-3ba71cb58f83, 172.23.0.1#53
    Nov 24 15:51:15 sodi9.store named[801]: listening on IPv4 interface br-54a515f28da8, 172.24.0.1#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface br-6e4d6813981a, fe80::42:93ff:fea8:ed11%7#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface br-d7c58f5a5c3c, fe80::42:29ff:fef2:48b7%11#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface br-3ba71cb58f83, fe80::42:5fff:fe28:e737%13#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface veth90690c0, fe80::24fa:a4ff:fe88:79b4%16#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface veth3d985da, fe80::f0da:fdff:fef6:6a86%18#53
    Nov 24 15:51:16 sodi9.store named[801]: listening on IPv6 interface veth99afd18, fe80::20e1:3aff:fea1:3b2c%20#53
    root@sodi9:/home/sangbinlee9#
    
    
    
    
















