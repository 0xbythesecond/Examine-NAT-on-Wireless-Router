# Examine NAT on Wireless Router
![Packet Tracer - Examine NAT on a Wireless Router](https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/2ad802db-fb8b-4d38-99d8-33ef7ed15b7c)




Lab/Lesson: Examine NAT on a Wireless Router using Packet Tracer

## Objective:
In this lab/lesson, I have examined NAT configuration on a wireless router using Packet Tracer. The main objectives were to understand the NAT setup, set up PCs to connect to the wireless router using DHCP, and observe the traffic flow with NAT translation across the network.

### Part 1: Examine the configuration for accessing the external network
In this part, I added a general PC and then proceeded to connect it to the wireless router using a straight-through cable. Once connected, I configured the PC to gather an IP address via DHCP and took note of the IP address of the default gateway. Then, I accessed the router's configuration page using a web browser and examined the Internet connection information.

<img width="700" alt="View Routers Configurations" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/694bff5a-5ae0-41b3-b295-5b71a04ec9ac"/>


### Part 2: Examine the configurations for accessing the internal network
In this part, I accessed the Local Network configuration within the router's status menu. I reviewed the address assigned to the internal network and examined the DHCP server information, including the range of IP addresses that can be assigned to connected hosts.

- <img width="500" alt="Status Internet IP Address (Provided by ISP)" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/97e4b8f5-9500-4b50-9b16-674c7485a520"/>

- <img width="500" alt="Range of IP Address that can be Assigned to Connected Host" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/fe32c4f4-7733-4040-af44-4b1a46355b4e"/>



### Part 3: Connect PCs to the wireless router
In this part, I added three more PCs and connected them to the wireless router using straight-through cables. I configured each PC to receive an IP address via DHCP. Finally, I verified the IP configurations of the PCs using the Command Prompt and the "ipconfig /all" command.

<img width="500" alt="ipconfig all pc3" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/0b7d71d6-ce6f-4b6e-bc80-8eb52da379e4"/>


  >**Note**: I understood that these devices would receive private addresses that cannot cross the internet, necessitating NAT translation.

### Part 4: View NAT translation across the wireless router
In this part, I entered Simulation mode and created a Complex PDU to view traffic. I set the source PC (PC0), specified the destination server (ciscolearn.net.com), and configured PDU settings such as the application and source port. By playing the simulation, I observed the traffic flow across the network with NAT translation.
![Adding Complex PDU](https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/d3157677-f5b9-47b8-880c-94670cb2c304)


  >**Note**: I adjusted the simulation speed and clicked "View Previous Events" when necessary provided below once the events reached their capacity.

### Part 5: View the header information of the packets that traveled across the network
In this part, I examined the headers of the packets sent between a PC and the web server. I accessed the Simulation Panel, selected an event, and viewed the packet and header information. I checked the Inbound and Outbound PDU details to observe the source (SRC) and destination IP addresses, noticing the change in the source IP address.
- Simulated Events
  - <img width="350" alt="image" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/f95db172-45ca-420d-8770-8210a487bddb"/>
- Inbound
  - <img width="500" alt="Inbound PDU Details" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/e29b80b5-3b3f-4115-b564-b6fb19b4d993"/>
- Outbound
  - <img width="500" alt="Outbound PDU Details" src="https://github.com/0xbythesecond/Examine-NAT-on-Wireless-Router/assets/23303634/d25c6a6f-b706-42f3-81e2-e82927257f3e"/>



  >**Note**: I navigated through other event lines to further analyze the headers.

## Conclusion:
By completing this lab/lesson, I successfully examined NAT configuration on a wireless router using Packet Tracer. I gained hands-on experience in setting up PCs to connect to the router, analyzing network configurations, and observing traffic flow with NAT translation. Understanding NAT is crucial for managing IP address allocations and enabling communication between private and public networks.
