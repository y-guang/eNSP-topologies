AR1

```bash
<Huawei>int	
<Huawei>sy	
<Huawei>system-view 
Enter system view, return user view with Ctrl+Z.
[Huawei]int g0/0/0
[Huawei-GigabitEthernet0/0/0]ip add	
[Huawei-GigabitEthernet0/0/0]ip address 172.16.0.254 255.255.255.0
[Huawei-GigabitEthernet0/0/0]
May  1 2023 08:15:31-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[0]:The line protocol
 IP on the interface GigabitEthernet0/0/0 has entered the UP state. 
[Huawei-GigabitEthernet0/0/0]q
[Huawei]int g0/0/1
[Huawei-GigabitEthernet0/0/1]ip address 119.1.1.1 255.255.255.0
[Huawei-GigabitEthernet0/0/1]
May  1 2023 08:16:35-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[1]:The line protocol
 IP on the interface GigabitEthernet0/0/1 has entered the UP state. 
[Huawei-GigabitEthernet0/0/1]
[Huawei-GigabitEthernet0/0/1]ip rou	
[Huawei-GigabitEthernet0/0/1]q
[Huawei]ip rou	
[Huawei]ip route-s	
[Huawei]ip route-static 200.200.200.0 255.255.255.0 119.1.1.2
[Huawei]int g0/0/1
[Huawei-GigabitEthernet0/0/1]nat server global 119.1.1.123 n	
[Huawei-GigabitEthernet0/0/1]nat server global 119.1.1.123 in	
[Huawei-GigabitEthernet0/0/1]nat server global 119.1.1.123 inside 172.16.0.1
[Huawei-GigabitEthernet0/0/1]
```

AR2

```bash
<Huawei>int	
<Huawei>sy	
<Huawei>system-view 
Enter system view, return user view with Ctrl+Z.
[Huawei]int g0/0/0
[Huawei-GigabitEthernet0/0/0]ip add	
[Huawei-GigabitEthernet0/0/0]ip address 119.1.1.2
                                                  ^
Error:Incomplete command found at '^' position.
[Huawei-GigabitEthernet0/0/0]ip address 119.1.1.2 255.255.255.255
Error: The specified IP address is invalid.
[Huawei-GigabitEthernet0/0/0]ip address 119.1.1.2 255.255.255.0
[Huawei-GigabitEthernet0/0/0]
May  1 2023 08:17:56-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[0]:The line protocol
 IP on the interface GigabitEthernet0/0/0 has entered the UP state. 
[Huawei-GigabitEthernet0/0/0]int g0/0/1
[Huawei-GigabitEthernet0/0/1]ip addr 200.200.200.200.254
                                     ^
Error: Wrong parameter found at '^' position.
[Huawei-GigabitEthernet0/0/1]ip addr 200.200.200.200.254 255.255.255.0
                                     ^
Error: Wrong parameter found at '^' position.
[Huawei-GigabitEthernet0/0/1]ip addr 200.200.200.254 255.255.255.0
[Huawei-GigabitEthernet0/0/1]
May  1 2023 08:18:52-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[1]:The line protocol
 IP on the interface GigabitEthernet0/0/1 has entered the UP state. 
[Huawei-GigabitEthernet0/0/1]
```

