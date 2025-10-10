# Financial_institution_project
This is a financial institution networking project 


Design and Implementation of a Financial Institution System Networking Project (Project #9)
Project #9 Case Study and Requirements
Download this Project

Jubilee Financial Services Ltd (JFSL) is a well-established finance service provider in Kenya, which offers online finance solutions and services to its clients. The company operates in the country’s capital city, Nairobi, and is hosted within an eleven-story building. The company primarily operates from the seventh to the eighth floors where on each floor there are at least two departments. The company has the following five departments within its main headquarter Human resource (HR), Customer Service (CS), Marketing (MK), Legal Management (LM), and Information Technology (IT). The number of users and other devices per department include;
1. Seventh Floor- HR, CS and MK; each department has at least 40 user devices plus 40 IP phones, and one WIFI-AP.
2. Eighth Floor- LM and IT; each department has at least 20 user devices plus 20 IP phones, and one WIFI-AP. N/B- each user can have an associated  VoIP phone (but not a must).
The network infrastructure is currently run and managed by a third-party firm called Infinitive IT Systems Kenya. The senior management has decided to own its network infrastructure including Local Area Network (LAN), Wide Area Network (WAN), and an external Server-Side location connected via appropriate WAN technology with prioritizing  secure communication between the HQ network and the external site. The server-side site will host DHCP, DNS, WEB, and EMAIL servers. The Company is intending to subscribe to two ISPs (Safaricom and JTL ISPs) to provide redundancy and load-balancing in terms of internet provisions. The company has also purchased two Cisco Catalyst 2911 routers (one for HQ and other for serverside) plus one gateway router Catalyst 2811 router(for HQ VoIP), two multilayer switches(both for HQ), and six access switches for the departments.
Due to security requirements, it has been decided that all five departments will be on a separate network segment within the same local area network. None of the servers is located within the local area network but will be hosted from an external site accessible via a WAN connection. The network security policy will comprehensively dictate the user access to the external site using Access Control LIST (ACL).

You have been hired as a network security engineer to design the network for Jubilee Financial Services Ltd (JFSL) according to the requirements set by the senior management. You will consult an appropriate robust network design model to meet the design requirements. You will also implement Access Control Lists and Virtual Private Networks to enable secure communication considering security and network performance factors paramount to safeguard the Confidentiality, Integrity, and Availability of data and communication.
The company has emphasized high performance, redundancy, scalability, and availability, and hence you are required to provide a complete JFSL network infrastructure design and implementation. The company will be using the following IP address: 192.168.20.0/24 for Data, 10.10.10.0/24 for Voice, and 190.200.100.0 for public addresses.
• Design Tool- Use Cisco Packet Tracer to design and implement the network solution.
• Hierarchical Design- Use a hierarchical model providing redundancy at every layer.
• ISPs- The network is also expected to connect to at least two ISPs to provide redundancy and each router is connected to the two ISPs.
• WIFI- Each department is required to have a wireless network for the users.
• VoIP- Each department should have IP phones and users in the department should be able to call each other.
• VLAN- Each department should be in a different VLAN and a different subnetwork. The voice VLAN ID number will remain at VID 120 for the entire network.
• Subnetting- Provided the networks above, carry out subnetting to allocate the correct number of IP addresses to each department.
• Basic settings- Configure basic device settings such as hostnames, and console passwords, enable passwords, and banner messages, encrypt all passwords and disable IP domain lookup.
• Inter-VLAN Routing- Devices in all the departments are required to communicate with each other with the respective multilayer switch configured for inter-VLAN routing.
• Core Switches- The Multilayer  switches are expected to carry out both routing and switching functionalities and thus will be assigned IP addresses.
• DHCP Server- All devices in the network (except IP phones) are expected to obtain an IP address dynamically from the dedicated DHCP servers located at the server-side site.
• Cisco 2811 Router- Ensure to have a  router that can support telephony service i.e Cisco Catalyst 2811(the VoIP router should be connected to any of the l3-switches at HQ).
• Static Addressing- Devices in the server room are to be allocated IP addresses statically.
• Telephony Service- Configure VoIP on the voice gateway router and allocate dial numbers in format (4..).
• Routing Protocol- Use OSPF as the routing protocol to advertise routes both on the routers and multilayer switches.
• Switchport security- Configure port security for the server site department switch to allow only one device to connect to a switch port, and use the sticky method to obtain mac-address and violation mode shutdown.
• SSH- Configure SSH in all the routers and layer three switches for remote login.
• Standard ACL for SSH- configure a simple standard ACL on the line VTY to allow only the ICT department to carry out all remote administrative tasks using SSH.
• NAT + ACL- Configure PAT to use the respective outbound router interface IPv4 address, and implement the necessary ACL rule.
• IPsec VPN + ACL- Configure site-to-site IPsec VPN between the HQ router and the Server-side router, and implement the necessary ACL rule.
• Final- Test Communication, ensure everything configured is working as expected.
Technologies Implemented
1. Creating a network topology using Cisco Packet Tracer.
2. Hierarchical Network Design.
3. Connecting Networking devices with Correct cabling.
4. Configuring Basic device settings.
5. Creating VLANs and assigning ports VLAN numbers.
6. Creating both data and voice VLANs and assigning ports VLAN numbers.
7. Subnetting and IP Addressing.
8. Configuring Inter-VLAN Routing both on the Switches (SVI) and Routers (router-on-a-stick).
9. Configuring Dedicated DHCP Server device for Data to provide dynamic IP allocation.
10. Configuring Routers as DHCP server for Voice to provide IP Phones dynamic IP allocation.
11. Configuring SSH for secure Remote access.
12. Configuring OSPF as the routing protocol.
13. Configuring Standard ACL for VTY interfaces to restrict remote Access using SSH.
14. Configuring Port Address Traslations or PAT for NAT.
15. Configuring Standard ACL for PAT.
16. Configuring VoIP or Telephony service configuration in all routers.
17. Configuring site-to-site IPsec VPN on the gateway routers.
18. Configuring Standard ACL for site-to-site IPsec VPN.
19. Host Device Configurations.
20. Test and Verifying Network Communication.
