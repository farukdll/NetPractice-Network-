<h1 align="right"> <a name="up"></a>

<h1 align="center"> NetPractice(Network Addressing)

<h1 align="center">
</br>
<p>
  <img width="150" alt="Host" src="https://user-images.githubusercontent.com/97880185/211656437-609c2afe-8673-4b69-b960-9a8247a855c3.png">
  <img width="160" alt="Switch" src="https://user-images.githubusercontent.com/97880185/211656464-3daa6f82-578b-4c6b-8d54-ff28b93e670f.png">
  <img width="150" alt="Router" src="https://user-images.githubusercontent.com/97880185/211656451-11235c84-f555-427b-916e-93a428a816b9.png">
  <img width="130" alt="Internet" src="https://user-images.githubusercontent.com/97880185/211656370-91ad141f-d7c5-4877-8136-0f7f6237c646.png">
</h1> <p> </p>


### Description
  * ###### NetPractice is a project that provides an understanding of networking concepts with a focus on solving TCP/IP addressing and network configuration problems. In this way, you will learn basic concepts such as IP addressing, subnet mask calculation, router and switch usage, while improving your network management skills.


### Table of Contents
  * [What is TCP/IP ?](#witcpip)
  * [What is TCP ?](#witcp)
  * [What is a IP ?](#wiaipadd)
  * [Binary number system calculation for IP addresses](#bnscfipaddss)
  * [What is the difference between TCP and IP ?](#witdbtcpaip)
  * [What are Network ID and Host ID ?](#wanidahid)
  * [What are Private and Public IP addresses?](#wapapipaddd)
  * [What is a Network address ?](#wianipadd)
  * [What is a Broadcast address ?](#wiabipadd)
  * [What is a switch ?](#wiasch)
  * [What is a router ?](#wiarer)
  * [How do switch and router work and what is the difference between them ?](#hasarwwitdbt)
  * [What is a diversion table ?](#wiadttle)
  * [Questions and Solutions](#quesaslti)


#### What is TCP/IP ? <a name="witcpip"></a>
  * ###### TCP/IP stands for Transmission Control Protocol/Internet Protocol and refers to a family of protocols that enable data communication over the Internet. This protocol family sets the standards and rules that make communication between computers possible. The TCP/IP protocol family includes many sub-protocols, such as IP (Internet Protocol) and TCP (Transmission Control Protocol), and is the foundation of the internet. IP is used for routing data packets and delivering them to the destination device, while TCP is used to ensure reliability in data communication. Together, the TCP/IP protocol family ensures reliable and efficient data communication over the internet.
  * ###### To summarize, the TCP/IP family of protocols is a generic structure for data communication over the Internet, consisting of four main layers: the application layer, which includes applications with which users interact directly; the transport layer, which provides reliability in data communication; the internet layer, which provides routing of data packets; and the network access layer, which provides physical network connectivity.
  * ###### If you want me to explain it in a simpler way, In the TCP/IP Protocol, there are 4 layers. At the top layer is the application layer. The application layer receives data from the user and processes it, converting it into data packets; such as web browsers, email clients, etc. Then it sends these packets to a lower layer, the transport layer. The transport layer receives these data packets and delivers them reliably to the next lower layer, the internet layer, reaching the destination. It also controls the data flow and performs error correction. The internet layer, in turn, receives the data packets from the transport layer and directs them to the next lower layer, the network access layer. Each device is assigned a unique IP address, and the packets are transmitted according to these addresses. The network access layer provides the physical network connection and transmits the data packets in binary format over the physical network; for example, using technologies like Ethernet or Wi-Fi.
  * ###### Here is a sample TCP/IP Protocol Diagram
  <h1 align="center">
  <p>
      <img height="280" width="450" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/733c2f9c-4bdd-4bdc-b814-fd74a5fb22be">
      <img height="280" width="350" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/13b44816-49cb-4daf-9441-8b9b3a89897a">
  </h1> <p> </p>


#### What is TCP ? <a name="witcp"></a>
  * ###### TCP (Transmission Control Protocol) is a communication protocol used to establish reliable connections between computers. TCP ensures secure packaging, sending, receiving, and reordering of data packets. This protocol operates on top of IP (Internet Protocol) and includes important features such as connection establishment, correct sequencing of data packets, error detection, and correction. These features provided by TCP ensure reliable and orderly data communication over the Internet.
  * ###### In simpler terms, TCP (Transmission Control Protocol) guarantees the integrity of data transmitted over a network. It establishes a connection between the source and destination before data transmission and maintains this connection until communication begins. It then divides large amounts of data into small packets during the data flow and ensures that it is delivered end-to-end without any data loss.
    * ###### TCP's main tasks at the layer where it resides are the following: Data Transmission, Flow Control, Error Correction, Connection Management.
    * ###### Data Transmission: TCP is responsible for reliably transmitting data packets between computers. It ensures that data packets are not lost and arrive at the destination intact.
    * ###### Flow Control: TCP regulates the flow of data. It adjusts the speed of data packets and controls traffic on the network, preventing overload.
    * ###### Error Correction: TCP detects and corrects errors that may occur in data packets. This maintains the integrity of the data packets.
    * ###### Connection Management: TCP establishes a connection before communication starts and closes the connection when communication ends. This ensures that data transmission takes place in a successful and orderly manner.
  <h1 align="center">
  <p>
      <img height="280" width="350" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/a6dc9757-fc20-4afa-b294-cfd09c947478">
      <img height="280" width="450" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/df2eac38-a7eb-4c19-8cee-5eefd57b9db8">
  </h1> <p> </p>


#### What is a IP ? <a name="wiaipadd"></a>
  * ###### IP (Internet Protocol) is a communications protocol used to enable data communication in computer networks. This protocol manages the routing, addressing and forwarding of data packets. IP enables communication between different devices on a network. IP resides at the Internet Layer, the third layer of the TCP/IP protocol stack. The Internet Layer handles the addressing and routing of data packets. IP works closely with TCP (Transmission Control Protocol) at the transport layer. TCP manages the flow of data while IP handles the addressing and routing of data packets. These two protocols work together to ensure reliable and accurate communication between computers.
  * ###### An IP address is a sequence of numbers separated by dots. IP addresses are expressed as a set of four numbers; an example address would be 192.158.1.38. Each number in the set can range from 0 to 255. So the full IP addressing range is from 0.0.0.0.0 to 255.255.255.255.255.
  * ###### IP's main tasks at the layer where it resides are the following: Addressing, Routing, Fragmentation, Error Detection, Protocol Management
  * ###### Addressing: IP assigns each device a unique address. This address determines the location of the device on the network and ensures that data packets reach the correct destination. These addresses can usually be in IPv4 or IPv6 format.
  * ###### Routing: IP routes data packets based on their source and destination addresses. This ensures that data packets reach the correct destination and manages communication on the network.
  * ###### Fragmentation: IP enables communication by dividing data packets into portable sizes (fragmentation) between different networks during transmission. This is necessary because different network technologies support different maximum data packet sizes.
  * ###### Error Detection: IP performs error detection to ensure the integrity of transmitted data packets. It detects erroneous or corrupted packets and sends an alert for retransmission if necessary.
  * ###### Protocol Management: Provides management of upper layer protocols such as IP, TCP and UDP. This determines which upper layer protocol data packets use and carries information about these protocols with the data packets.
  <h1 align="center">
  <p>
      <img height="280" width="350" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/947bc78c-0951-4ea2-9d97-961c6f775fe2">
      <img height="280" width="450" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/df2eac38-a7eb-4c19-8cee-5eefd57b9db8">
      <img height="180" width="800" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/87f5a6a6-bba1-42d3-a51e-fcbd450e0acf">
  </h1> <p> </p>
  
#### Binary number system calculation for IP addresses <a name="bnscfipaddss"></a>
  * ###### Let's calculate 192.168.11.10 sample ip address in binary → 11000000.10101000.00001011.00001010
  * ###### 192
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/5a4305fc-84eb-409c-8e35-ba2d42095ea7">
  </h1> <p> </p>
  
  * ###### 168
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/4ff7e2b3-6563-4b69-8634-7ad82b5c7332">
  </h1> <p> </p>
  
  * ###### 11
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/52b2998a-bd92-4075-98f0-f6f2a2cfbbe2">
  </h1> <p> </p>
  
  * ###### 10
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/be1fb690-be8d-4971-b064-6ff7edfa2fa8">
  </h1> <p> </p>


#### What is the difference between TCP and IP ? <a name="witdbtcpaip"></a>
  * ###### TCP and IP are two separate computer network protocols.
    * ###### TCP (Transmission Control Protocol):
      * ###### TCP is a communication protocol used to ensure reliable communication between computers.
      * ###### It manages the data flow, sorts data packets, performs error correction and provides flow control.
      * ###### It is a connection-based protocol; it manages connection establishment, data exchange and connection termination.
      * ###### It is located at the Transport Layer and works together with IP to form the second layer for data transmission.
    * ###### IP (Internet Protocol):
      * ###### IP is responsible for addressing and routing data packets in computer networks.
      * ###### Thanks to IP addresses, computers find each other and perform data flow.
      * ###### It is located at the Internet Layer and forms the third layer of the TCP/IP protocol stack.
      * ###### It routes data packets according to source and destination addresses and thus enables communication.
      * ###### Identifies devices with unique addresses, usually in IPv4 or IPv6 format.


#### What are Network ID and Host ID ? <a name="wanidahid"></a>
  * ###### Network ID :
    * ###### The network ID of an IP address indicates that all devices on the network belong to a common network.
    * ###### The network ID represents the first parts of the IP address in a particular network. This indicates that all devices on the network share the same network and belong to the same network.
  * ###### Host ID :
    * ###### The host ID is the unique identifier of devices on a given network and each device has its own unique ID.
    * ###### Each device utilizes its unique identifier to communicate with other devices on the network.
  * ###### To summarize, the Network ID represents the general location of an IP address within a network, while the Host ID represents the unique identity of a specific device within this network. In other words, Network ID and Host ID form the basis of the inter-network communication and addressing systems of IP addresses.
  <h1 align="center">
  <p>
      <img height="130" width="500" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/5b40110b-0ad0-4416-ae52-5c1941b4f651">    
  </h1> <p> </p>


#### What are Private and Public IP addresses ? <a name="wapapipaddd"></a>
  * ###### Public IP addresses :
    * ###### Public IP addresses are the unique identifier of a device on the internet and are used to communicate with other internet users or devices.
    * ###### Public IP addresses are IP addresses that are open to the internet and accessible worldwide. Public IP addresses are used for websites, servers, network devices and other internet accessible devices.
    * ###### Public IP addresses are obtained by internet service providers from IANA (Internet Assigned Numbers Authority) or other authorized organizations. 
    * ###### Public IP addresses are usually globally unique as they are accessible over the internet and are used to identify millions of individual devices.  This means that they are unique across all devices connected to the internet and are therefore considered a limited resource.
    <h1 align="center">
    <p>
        <img height="400" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/f5bd2d42-b7d0-4657-a56a-de8a248857c6">
    </h1> <p> </p>

  * ###### Private IP addresses :
    * ###### Private IP addresses are IP addresses that are used on a private network and are not accessible over the internet.
    * ###### These addresses are used to communicate between devices within private networks.
    * ###### Private IP addresses are not assigned by IANA or other authoritative organizations; instead, they are assigned by a specific network administrator.
    * ###### We cannot use private IP addresses directly on the internet because they are designed for use in closed networks that are not directly accessible to the internet. These addresses are only used for communication between devices within a specific network and are not intended for internet traffic.
    * ###### Finally, the range 127.0.0.0.0 - 127.255.255.255.255 is reserved for a special IP address "localhost". This IP address represents the self-connection of a device and usually refers to the local loopback interface of the computer. This address is usually used for local testing and development purposes and is not accessible over the internet. Therefore, this address is also one of the private IP addresses.
    <h1 align="center">
    <p>
        <img height="140" width="500" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/4435cb8d-8ab8-4bd7-824e-6e6fb8164a27">
    </h1> <p> </p>



#### What is a Network address ? <a name="wianipadd"></a>


#### What is a Broadcast address ? <a name="wiabipadd"></a>


#### What is a switch ? <a name="wiasch"></a>


#### What is a router ? <a name="wiarer"></a>


#### How do switch and router work and what is the difference between them ? <a name="hasarwwitdbt"></a>


#### What is a diversion table ? <a name="wiadttle"></a>


#### Questions and Solutions : <a name="quesaslti"></a>
<details>
  <summary>Level 1</summary>
  <br>
  <img width="1223" alt="Level-1" src="https://user-images.githubusercontent.com/97880185/212213694-7524003c-d261-4f73-ae1b-df7a0012a9ac.png">
  <br> 
</details>

---
<details>
  <summary>Level 2</summary>
  <br>
  <img width="1223" alt="Level-2" src="https://user-images.githubusercontent.com/97880185/212213738-7536bda7-3bbf-4910-95d1-d689836d0856.png"> 
  <br>
</details>

---
<details>
  <summary>Level 3</summary>
  <br>
  <img width="1223" alt="Level-3" src="https://user-images.githubusercontent.com/97880185/212213866-f30c18c5-5ad7-4205-a0c1-b915e0293dcd.png">
  <br>
</details>

---
<details>
  <summary>Level 4</summary>
  <br>
  <img width="1223" alt="Level-4" src="https://user-images.githubusercontent.com/97880185/212213928-5cec0a99-ce40-4f20-89d7-2368cdde68ba.png">
  <br> 
</details>

---
<details>
  <summary>Level 5</summary>
  <br>
  <img width="1321" alt="Level-5" src="https://user-images.githubusercontent.com/97880185/212213967-74620659-7f35-40ef-ad5e-bf7c4d420045.png">
  <br>
</details>

---
<details>
  <summary>Level 6</summary>
  <br>
  <img width="1241" alt="Level-6" src="https://user-images.githubusercontent.com/97880185/212214010-98d800ca-b6af-4876-8bdd-6f95b66ce1b5.png">
  <br>
</details>

---
<details>
  <summary>Level 7</summary>
  <br>
  <img width="1419" alt="Level-7" src="https://user-images.githubusercontent.com/97880185/212214041-19c5b633-6f48-4a15-90e4-387a1a344180.png">
  <br> 
</details>

---
<details>
  <summary>Level 8</summary>
  <br>
  <img width="1126" alt="Level-8" src="https://user-images.githubusercontent.com/97880185/212214101-7c97ee4e-791d-454a-8a23-54a15be54024.png">
  <br>
</details>

---
<details>
  <summary>Level 9</summary>
  <br>
  <img width="1101" alt="Level-9" src="https://user-images.githubusercontent.com/97880185/212214179-ac1a2755-4994-46e4-bed1-a2fef5b4913f.png">
  <br>
</details>

---
<details>
  <summary>Level 10</summary>
  <br>
  <img width="1124" alt="Level-10" src="https://user-images.githubusercontent.com/97880185/212214241-bcca2d94-e5dd-4f18-a8be-eb9bc1b89794.png">
  <br>
</details>

---










|[ ⬆︎  Up](#up)|
|      :-:     |
