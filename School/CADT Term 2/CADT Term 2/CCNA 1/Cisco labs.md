# 1.0.5
asl2 wired connections are access point, asl1 and webserver
laptop is connected to access point 

laptop is on the table
asl2 is in the server rack

# 1.5.5

endpoint: printer, laptop, pc, tablet, phone, server

5


# Practical lab 4/7/25

## topology 

### VLAN10 Guest

- IP Range: 192.168.0.0/24

- F0/1-F0/5

### VLAN20 Student

- IP Range: 192.168.1.0/24

- F0/6-F0/10

### VLAN30 Staff

- IP Range: 192.168.2.0/24
- F0/11-F0/15


en
config t
vlan 10
name guest
vlan 20
name student
vlan 30
name staff

interface f0/1-5
switchport mode access
switch access

password: password
enable secret: secret

switch 1, local user
Username: admin
Password: admin



https://securitywithblue.medium.com/ssh-configuration-on-cisco-switch-f138535391eb

https://www.cisco.com/c/en/us/td/docs/switches/lan/catalyst2960x/software/15-0_2_EX/vlan/configuration_guide/b_vlan_152ex_2960-x_cg/b_vlan_152ex_2960-x_cg_chapter_011.html,

