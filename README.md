# Cisco Wireless DHCP-Client 
Repository Title : Simulation of Wireless DHCP Client in Cisco Packet Tracer

Description : This simulation aims to visualize the concept of using a wireless connection with a DHCP Client. There are six rooms, each equipped with two computers, three laptops, two tablets, two smartphones, and two printers. All these devices are connected to a wireless network using the Access Point. The simulation is designed to demonstrate the functions and configuration of wireless connections in an office network environment.


## Designed Network
![Design Cisco](https://github.com/Alizaaaja4/Cisco_Wireless_DHCP-Router_Office/blob/main/Dokumentasi.jpeg)

### Devices Used
  - 3 Computers (PC)
  - 2 Access Point PT 
  - 2 Laptop
  - 2 Smartphones
  - 2 Printer PT
  - 2 Switch 2950-24
  - 1 Tablet
  - 1 Router 1841

## DHCP Client
DHCP client is a software or hardware device on a computer network that automatically sends requests to obtain IP address configurations and other network information from a DHCP server. The DHCP client is used to dynamically configure IP addresses and other network settings, allowing devices to connect to the network without manual configuration.

    Router> enable
    Router# configure terminal
    Router(config-if)# interface (ex: fa0/0)
    Router(config-if)# no shutdown
    Router(config-if)# ip address (ex: 192.168.10.1 ) subnetmask
    Router(config-if)# ip dhcp pool (ex: WIrelles1)
    Router(dhcp-config)# default-router (ex: 192.168.10.1)
    Router(dhcp-config)# network (ex: 192.168.10.0) 255.255.255.0
    Router(dhcp-config)# dns-server (ex: 8.8.8.8)
    
