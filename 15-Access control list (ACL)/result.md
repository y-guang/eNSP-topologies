LSW1

```bash
The device is running!

<Huawei>sy	
<Huawei>system-view 
Enter system view, return user view with Ctrl+Z.
[Huawei]vl	
[Huawei]vlan 30
[Huawei-vlan30]
Apr 30 2023 06:13:26-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 1, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-vlan30]q
[Huawei]int	
[Huawei]interface g0/0/4
[Huawei-GigabitEthernet0/0/4]set	
[Huawei-GigabitEthernet0/0/4]po	
[Huawei-GigabitEthernet0/0/4]port lin	
[Huawei-GigabitEthernet0/0/4]port link-t	
[Huawei-GigabitEthernet0/0/4]port link-type ac	
[Huawei-GigabitEthernet0/0/4]port link-type access 
[Huawei-GigabitEthernet0/0/4]por	
[Huawei-GigabitEthernet0/0/4]port ac
Apr 30 2023 06:14:16-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 2, th
e change loop count is 0, and the maximum number of records is 4095.c	
[Huawei-GigabitEthernet0/0/4]port acc	
[Huawei-GigabitEthernet0/0/4]port acc	
[Huawei-GigabitEthernet0/0/4]port acce	
[Huawei-GigabitEthernet0/0/4]pro	
[Huawei-GigabitEthernet0/0/4]por	
[Huawei-GigabitEthernet0/0/4]port d	
[Huawei-GigabitEthernet0/0/4]port de	
[Huawei-GigabitEthernet0/0/4]port default v	
[Huawei-GigabitEthernet0/0/4]port default vlan 3	
[Huawei-GigabitEthernet0/0/4]port default vlan 30
[Huawei-GigabitEthernet0/0/4]
Apr 30 2023 06:17:26-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 3, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-GigabitEthernet0/0/4]q
[Huawei]interface g0/0/2
[Huawei-GigabitEthernet0/0/2]display this
#
interface GigabitEthernet0/0/2
 port link-type access
 port default vlan 10
#
return
[Huawei-GigabitEthernet0/0/2]q
[Huawei]q
<Huawei>save
The current configuration will be written to the device.
Are you sure to continue?[Y/N]y
Now saving the current configuration to the slot 0.
Apr 30 2023 06:23:20-08:00 Huawei %%01CFM/4/SAVE(l)[0]:The user chose Y when dec
iding whether to save the configuration to the device.
Save the configuration successfully.
<Huawei>
<Huawei>sy
Enter system view, return user view with Ctrl+Z.
[Huawei]int	
[Huawei]interface g0/0/4
[Huawei-GigabitEthernet0/0/4]display thi	
[Huawei-GigabitEthernet0/0/4]display this 
#
interface GigabitEthernet0/0/4
 port link-type access
 port default vlan 30
#
return
```



LSW2

```bash
The device is running!

<Huawei>display this
#
return
<Huawei>sy
Enter system view, return user view with Ctrl+Z.
[Huawei]display this
#
sysname Huawei
#
vlan batch 10 20
#
cluster enable
ntdp enable
ndp enable
#
drop illegal-mac alarm
#
return
[Huawei]vlan 30
[Huawei-vlan30]vlan 20
[Huawei-vlan20]dis
Apr 30 2023 06:19:28-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 1, th
e change loop count is 0, and the maximum number of records is 4095.p	
[Huawei-vlan20]display t	
[Huawei-vlan20]display this
#
return
[Huawei-vlan20]q
[Huawei]display this
#
sysname Huawei
#
vlan batch 10 20 30
#
cluster enable
ntdp enable
ndp enable
#
drop illegal-mac alarm
#
return
[Huawei]inter	
[Huawei]interface V	
[Huawei]interface Vlanif 30
[Huawei-Vlanif30]
Apr 30 2023 06:20:27-08:00 Huawei %%01IFNET/4/IF_STATE(l)[0]:Interface Vlanif30 
has turned into UP state.
[Huawei-Vlanif30]ip add	
[Huawei-Vlanif30]ip address 3.3.3.254 255.255.255.0
[Huawei-Vlanif30]
Apr 30 2023 06:20:45-08:00 Huawei %%01IFNET/4/LINK_STATE(l)[1]:The line protocol
 IP on the interface Vlanif30 has entered the UP state.
[Huawei-Vlanif30]
Apr 30 2023 06:20:48-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 2, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-Vlanif30]q
[Huawei]q
<Huawei>save
The current configuration will be written to the device.
Are you sure to continue?[Y/N]y
Now saving the current configuration to the slot 0.
Apr 30 2023 06:23:11-08:00 Huawei %%01CFM/4/SAVE(l)[2]:The user chose Y when dec
iding whether to save the configuration to the device.
Save the configuration successfully.
<Huawei>acl name PC3AccessControl
        ^
Error: Unrecognized command found at '^' position.
<Huawei>sy	
<Huawei>system-view 
Enter system view, return user view with Ctrl+Z.
[Huawei]acl name PC3AccessControl ?
  INTEGER<2000-2999>  Basic access-list(add to current using rules)
  INTEGER<3000-3999>  Advanced access-list(add to current using rules)
  INTEGER<4000-4999>  Specify a L2 acl group
  INTEGER<5000-5999>  User defined access-list
  advance             Advanced ACL
  basic               Basic ACL
  link                Link ACL
  user                User ACL
  <cr>                

[Huawei]acl name PC3AccessControl adv	
[Huawei]acl name PC3AccessControl advance
[Huawei-acl-adv-PC3AccessControl]
Apr 30 2023 06:25:28-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 3, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-acl-adv-PC3AccessControl]reule de	
[Huawei-acl-adv-PC3AccessControl]rule dy	
[Huawei-acl-adv-PC3AccessControl]rule den	
[Huawei-acl-adv-PC3AccessControl]rule deny ip so	
[Huawei-acl-adv-PC3AccessControl]rule deny ip source 1.1.1.0 0.0.0.255
[Huawei-acl-adv-PC3AccessControl]
Apr 30 2023 06:28:38-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 4, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-acl-adv-PC3AccessControl]display this
#
acl name PC3AccessControl 3999
 rule 5 deny ip source 1.1.1.0 0.0.0.255
#
return
[Huawei-acl-adv-PC3AccessControl]un	
[Huawei-acl-adv-PC3AccessControl]undo 	
[Huawei-acl-adv-PC3AccessControl]undo deny ip source 1.1.1.0 0.0.0.255
                                      ^
Error: Unrecognized command found at '^' position.
[Huawei-acl-adv-PC3AccessControl]undo rule deny ip source 1.1.1.0 0.0.0.255
                                           ^
Error: Wrong parameter found at '^' position.
[Huawei-acl-adv-PC3AccessControl]undo ?
  configuration  Configuration interlock
  debugging      Enable system debugging functions
  description    Specify ACL description
  rule           Specify an ACL rule
  screen-width   Set screen width
  step           Specify step of ACL sub rule ID

[Huawei-acl-adv-PC3AccessControl]undo ru	
[Huawei-acl-adv-PC3AccessControl]undo rule ?
  INTEGER<0-4294967294>  ID of ACL rule

[Huawei-acl-adv-PC3AccessControl]undo rule 5
[Huawei-acl-adv-PC3AccessControl]display this
#
acl name PC3AccessControl 3999
#
return
[Huawei-acl-adv-PC3AccessControl]undo rule deny ip source 1.1.1.0 0.0.0.255
Apr 30 2023 06:30:38-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 5, th
e change loop count is 0, and the maximum number of records is 4095.	
[Huawei-acl-adv-PC3AccessControl]undo rule deny ip source 1.1.1.0 0.0.0.255 de	
[Huawei-acl-adv-PC3AccessControl]undo rule deny ip source 1.1.1.0 0.0.0.255 des	

[Huawei-acl-adv-PC3AccessControl]undo rule deny ip source 1.1.1.0 0.0.0.255 de	
[Huawei-acl-adv-PC3Acrule deny ip source 1.1.1.0 0.0.0.255 de	
[Huawei-acl-adv-PC3AccessControl]rule deny ip source 1.1.1.0 0.0.0.255 destinati
on 3.3.3.0 0.0.0.255
[Huawei-acl-adv-PC3AccessControl]rule ip
Apr 30 2023 06:32:08-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 6, th
e change loop count is 0, and the maximum number of records is 4095	
[Huawei-acl-adv-PC3AccessControl]rule per	
[Huawei-acl-adv-PC3AccessControl]rule permit ip sou	
[Huawei-acl-adv-PC3AccessControl]rule permit ip source an	
[Huawei-acl-adv-PC3AccessControl]rule permit ip source any de	
[Huawei-acl-adv-PC3AccessControl]rule permit ip source any destination a	
[Huawei-acl-adv-PC3AccessControl]rule permit ip source any destination any 
[Huawei-acl-adv-PC3AccessControl]display th
Apr 30 2023 06:32:38-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 7, th
e change loop count is 0, and the maximum number of records is 4095.i	
[Huawei-acl-adv-PC3AccessControl]display this 
#
acl name PC3AccessControl 3999
 rule 5 deny ip source 1.1.1.0 0.0.0.255 destination 3.3.3.0 0.0.0.255
 rule 10 permit ip
#
return
[Huawei-acl-adv-PC3AccessControl]q
[Huawei]int	
[Huawei]interface g0/0/1
[Huawei-GigabitEthernet0/0/1]tr	
[Huawei-GigabitEthernet0/0/1]traffic-filter inb	
[Huawei-GigabitEthernet0/0/1]traffic-filter inbound acl ?
  INTEGER<2000-2999>  Basic access-list
  INTEGER<3000-3999>  Advanced access-list
  INTEGER<4000-4999>  L2 access-list
  INTEGER<5000-5999>  User-defined access-list
  ipv6                Specify IPv6 
  name                Specify a named ACL 

[Huawei-GigabitEthernet0/0/1]traffic-filter inbound acl nam	
[Huawei-GigabitEthernet0/0/1]traffic-filter inbound acl name ?
  STRING<1-32>  Specify acl name 

[Huawei-GigabitEthernet0/0/1]traffic-filter inbound acl name PC3	
[Huawei-GigabitEthernet0/0/1]traffic-filter inbound acl name PC3AccessControl
[Huawei-GigabitEthernet0/0/1]
Apr 30 2023 06:34:49-08:00 Huawei DS/4/DATASYNC_CFGCHANGE:OID 1.3.6.1.4.1.2011.5
.25.191.3.1 configurations have been changed. The current change number is 8, th
e change loop count is 0, and the maximum number of records is 4095.
[Huawei-GigabitEthernet0/0/1]Vlanif 30
                             ^
Error: Unrecognized command found at '^' position.
[Huawei-GigabitEthernet0/0/1]q
[Huawei]Vlanif 30
        ^
Error: Unrecognized command found at '^' position.
[Huawei]inte	
[Huawei]interface vl	
[Huawei]interface Vlanif 30
[Huawei-Vlanif30]display this
#
interface Vlanif30
 ip address 3.3.3.254 255.255.255.0
#
return
[Huawei-Vlanif30]
```

