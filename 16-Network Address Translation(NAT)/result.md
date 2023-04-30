AR1

```bash

<Huawei>inte	
<Huawei>sy	
<Huawei>system-view 
<Huawei>system-view 
Enter system view, return user view with Ctrl+Z.
[Huawei]itner	
[Huawei]inte	
[Huawei]interface G0/0/0
[Huawei-GigabitEthernet0/0/0]ip addr	
[Huawei-GigabitEthernet0/0/0]ip address 192.168.1.25	
[Huawei-GigabitEthernet0/0/0]ip address 192.168.1.254 255.255.255.0
[Huawei-GigabitEthernet0/0/0]
Apr 30 2023 22:12:56-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[0]:The line protocol
 IP on the interface GigabitEthernet0/0/0 has entered the UP state. 
[Huawei-GigabitEthernet0/0/0]
[Huawei-GigabitEthernet0/0/0]interface G0/0/1
[Huawei-GigabitEthernet0/0/1]ip address 64.1.1.1 255.255.255.0
[Huawei-GigabitEthernet0/0/1]
Apr 30 2023 22:13:53-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[1]:The line protocol
 IP on the interface GigabitEthernet0/0/1 has entered the UP state. 
[Huawei-GigabitEthernet0/0/1]q
[Huawei]
[Huawei]acl name LAN
[Huawei-acl-adv-LAN]q
[Huawei]redo acl name LAN
        ^
Error: Unrecognized command found at '^' position.
[Huawei]undo acl name LAN
[Huawei]acl name LAN bas	
[Huawei]acl name LAN basic 
[Huawei-acl-basic-LAN]rule per	
[Huawei-acl-basic-LAN]rule permit sour	
[Huawei-acl-basic-LAN]rule permit source 192.168.0.0 255.255.0.0
[Huawei-acl-basic-LAN]nat add	
[Huawei-acl-basic-LAN]nat addr	
[Huawei-acl-basic-LAN]q
[Huawei]
[Huawei]nat add	
[Huawei]nat address-group ?
  INTEGER<0-7>  Index of address-group
[Huawei]nat address-group 1 ?
  IP_ADDR<X.X.X.X>  Start address
[Huawei]nat address-group 1 64.1.1.2 ?
  IP_ADDR<X.X.X.X>  End address
[Huawei]nat address-group 1 64.1.1.2 64.1.1.6
[Huawei]int g0/0/1
[Huawei-GigabitEthernet0/0/1]nat out	
[Huawei-GigabitEthernet0/0/1]nat outbound 
[Huawei-GigabitEthernet0/0/1]nat outbound ?
  INTEGER<2000-3999>  Apply basic or advanced ACL
[Huawei-GigabitEthernet0/0/1]dis acl all
 Total quantity of nonempty ACL number is 1 

Basic ACL LAN 2999, 1 rule
Acl's step is 5
 rule 5 permit source 0.0.0.0 255.255.0.0 

[Huawei-GigabitEthernet0/0/1]nat ou	
[Huawei-GigabitEthernet0/0/1]nat outbound 	
[Huawei-GigabitEthernet0/0/1]nat outbound ?
  INTEGER<2000-3999>  Apply basic or advanced ACL
[Huawei-GigabitEthernet0/0/1]nat outbound 2999 add	
[Huawei-GigabitEthernet0/0/1]nat outbound 2999 address-group 1
[Huawei-GigabitEthernet0/0/1]q
[Huawei]acl name LAN
[Huawei-acl-basic-LAN]display all
                              ^
Error: Wrong parameter found at '^' position.
[Huawei-acl-basic-LAN]display this
[V200R003C00]
#
acl name LAN 2999  
 rule 5 permit source 0.0.0.0 255.255.0.0 
#
return
[Huawei-acl-basic-LAN]redo rule 5
                      ^
Error: Unrecognized command found at '^' position.
[Huawei-acl-basic-LAN]do rule 5un
[Huawei-acl-basic-LAN]undo rule 5
 Warning: The ACL sub item number does not exist!
[Huawei-acl-basic-LAN]rule ?
  INTEGER<0-4294967294>  ID of ACL rule
  deny                   Specify matched packet deny
  permit                 Specify matched packet permit
[Huawei-acl-basic-LAN]rule per	
[Huawei-acl-basic-LAN]rule permit sou	
[Huawei-acl-basic-LAN]rule permit source 192.168.0.0 0.0.255.255
```

AR2

```bash
<Huawei>sy
Enter system view, return user view with Ctrl+Z.
[Huawei]in	
[Huawei]int	
[Huawei]interface g0/0/0
[Huawei-GigabitEthernet0/0/0]ip addr 64.1.1.10 255.255.255.0
[Huawei-GigabitEthernet0/0/0]
Apr 30 2023 22:15:48-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[0]:The line protocol
 IP on the interface GigabitEthernet0/0/0 has entered the UP state. 
[Huawei-GigabitEthernet0/0/0]
```

