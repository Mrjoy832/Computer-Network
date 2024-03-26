# ✅🚀 Computer-Network(CN):
- [Tuitorial Link](https://youtu.be/IPvYjXCsTg8?si=w90vZx10j3cGVEMq)
- **ARPA**--> Advance Research Project Agency.
- ARPANET, basically 4 places where computer works--> MIT , Standford , UCLA , Utah univeristy

![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/6201af21-917f-4ad7-8aa6-f8cc8485365f)

- Diff types of rules are there to sent diff types of files into the internet , is called **Protocols**<br>
TCP=Transmission Control Protocol(data will reach destination and will not be corrupted in the way)<br>
UDP(User datagram protocol)=dont care all data will reach in once<br>
HTTP=Hyper Text Transfer Protocol(used by web browsers)

- **Server**:

![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/531e7628-d137-4794-be89-9f2fb9b87b59)

<br>
-  check IP of own machine ```curl ifconfig.me -s```
- ISP(internet service provider) like Airtel provides router which has global IP , all devices connected with the router has same IP , these are known as local IP. Routers are assigned to global IP with DHCP protocols. if u request for google.com from any connected machine google see the reuqest made by global IP. then google send back response to router or Global IP and later the Router decides whom to sent the request using NAT(Network Access Translator). Now we have to decide which application on that machine is requesting for the service...so have to decide where to sent the result on that machine. IP address decides which machine to sent the result data but the **Port num**  decides which application data should be sent. Port is 16 bit number , each bit contains 0/1...so total num of port availavale 2^16 = almost 65K. 
<br>All http stuffs done in PORT 80. MongoDB runs on 2707. <br>
0-1023 ports are reserved..<br>
1024-49152 are reserved for applications and the remaining ones we can use. <br>

## How does communication occurs btw 2 computer?
- Guided(by wires)--> optical fibre cable , coaxial cable
- Non Guided(bluetooth, wifi)

---

- **LAN**= local area network => house , office or in an particular area via Ethernet cable/wifi
- **WAN** = Accross countries=> optical fibre cables
- **MAN** = 

---
 - **Modems**=> used to convert digital to analog singals and vice versa.
 - **Router**==> routes data based on their IP address
---
#### How computers are connected?
- **Topologies**:
- 1. BUS Topology:
  2. Ring Topology
  3. Star Topology
  4. Tree topology
  5. Mesh Topology
   
---

## ✅OSI Model:(Structure of Network:) Open System Interconnection Model:
- How servers communicate with each others
- There are 7 layers ---> **APplication**[its implemented in software...users use these...this layer conatins application] , <br>
**presentation**[users data goes to this layer from application layer..converst our msg to machine readble binary formats and goes under encoding/encryption] ,<br>
**session**[helps in setting up connection and termination of the sessions] ,<br> **transport**[data transferred from session to transport...data recieved from sessions will be divided into small segments which will have seperate src and dest PORT num, also take part in err control and checksum] ,<br>
**Network**[works for transmission of recieved data btw computers situated between diff networks..routers live here, Logical Addressing/IP addressing here] ,<br>  **data link**[allows to directly communicate to computers...conatins IP of both sender and reciever machines in the form of packets] , <br> **Physical layer**[].

### [OSI from another Resource:](https://youtu.be/sCYkeo466Qs?si=2XhU6wvVmB7elec4) 

![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/fbec81b1-8fe4-4502-85b7-d74923a2256e)

Data ssending from client from Application to Physical(Top to buttom) but recieving into server from buttom to top(Physical to APplication)<br>

#### Example with Army Ranking:

![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/3390305a-b25c-4e95-a188-e75f81284374)

![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/0ef2da67-e550-41aa-aa0c-5be47195f891)

- in **Application layer** close to end user, user interact in this...when we browse anything , protocols HTTP. 
- In **Presentation Layer** , compresses the data and encrypt the data
- In **Session layer** open session btw sender and reciever and create Authentication
- In **transport layer**, heart of OSI , ensures perfect delivery of transporting the data , TCP,UDP lies here. Transport header (PORT )added ,
- In **network layer**, segement breaks into Packet...network header(Logical IP of dest) added. Router comes into this.
- **Data link**, ensures goes to dest err free and in a sequence, pacets divided into frames including the MAC address using ethernet
- **Physical LAyer**, netowrk physical cables reside ...binary bits data goes through the cables.

---
### ➡️TCP/IP Model
![image](https://github.com/Mrjoy832/Computer-Network/assets/77873383/767414d4-b09b-43ba-8b56-b85ef41fc39e)

- Application , presentation , session layer merged into Application layer
- DataLink and Physcial merged into Physical
- Rest all the functionalities are almost similar.
---

#### Read from anywhere:
- Repeator , Hub , Bridge , Switch , Routers, Gateway

---
## Protocols: 
- **TCP/IP**
 <br> **protocols under TCP/IP**:HTTP, DHCP , FTP , SMTP , POP3 , IMAC , SSH , VNC

- Telnet Protocol --> via port:23
- UDP --> stateless connection , data may be lost

----

