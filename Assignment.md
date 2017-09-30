Question 1:

The minimum seek time for an HDD is 9 msec, and the maximum seek time is 90 msec. The block size of this HDD is 4KB. How long on average does it take to read 100MB of data?

Answer :
<!--
Seek: To read from HDD, it's disk arm move to the correct track in this process.(From: http://pages.cs.wisc.edu/~remzi/OSFEP/file-disks.pdf)
In general the average seek time is taken as the average time, but the average seek time arises from calculating average seek distance.The average seek distance on a disk over all possible seeks is calculated as 1/3 rd of the full distance.Thus the average seek is one-third of a full seek.-->

Read time is calculated as: (Seek Time + Rotational Latency + Transfer Time)

// Cannot figure out this one 


QUESTION 2:

Describe a TCP/IP packet in detail. Describe the header, how many bytes it is, and which components it contains. What data can come after the header?

ANSWER :

TCP/IP is a set of rules for communication between devices on the internet.TCP/IP require information to be split into segment of data and address.It was created by Defense Advanced Research Projects Agency(DARPA) in 1970.

TCP/IP is based on client/server model of communication where both are in the network, the user requests and the server provides the service for the request being made.A packet is basic unit of information in network transmission.TCP/IP classified as stateless and considered as a packet-switching technology.The packets are constructed of two major parts:
1) the packet header,
2) the data.

Header:
The header contains distinct information about the packet.The header size ranges from 20-60 bytes where 20bytes being minimum and 60 bytes the maximum.The informations in the header are:
i) version of the protocol: like IPv4 or IPv6,
ii) length of the packet,
iii) address of source and destination: 16 bits each,
iv) checksum: used in error correction calculation (16 bits),
v) Time To Live(TTL) data: defines how many devices the packet may be transmitted along before it is allowed to time out.

Data:
The data is divided into segments of length.The length range from 0 to 64 KB.


QUESTION 3:

How does the network protocol guarantee that a TCP/IP packet is complete after transmission?

ANSWER:

TCP/IP 's each packet includes the source and destination address, which helps in delivering packets successfully but if some packets are missing then information can be sent and the packet gets retransmitted. The header information describes the version, length of packet, checksum, and other information which helps in reconstruction and correction of message.It also make the data transmission fast and reliable.


QUESTION 4:

What is the difference between TCP and IP?

ANSWER:

TCP: Transmission Control Protocol
1) It is a transport layer protocol.
2) It is a connection oriented and reliable protocol.
3) It provides the delivery of a stream of data from one computer to another computer in the form of packets.
4) It controls size, flow control, the rate of data exchange, and network traffic congestion.

IP: Internet Protocol
1) It is a network layer protocol.
2) It is a connection less protocol.
3) It defines addressing methods and structures for the encapsulation of the packets.
4) It is responsible for delivering distinguished protocol datagrams (also known as packets) from the source to the destination based only their addresses.


QUESTION 5:

Why is 3d performance so much higher with a graphics card than without? Modern CPUs are extremely fast, what is limiting their performance?

ANSWER:

Graphics card with their GPU(Graphics Processor Unit) are designed to handle complicated calculation related to 2D and 3D graphics.They are better at rendering certain calculations compared to CPU.On the other hand CPU is the heart of the computer where most calculations take place.But are restricted to certain mathematical calculations which require longer processing time.

Modern CPU are extremely fast which help to do the work faster on computer but following are the limitations to its performance:
i) COST:
   The faster processor comes with a high price.

ii) HEAT:
   Faster processor generate more heat and needs more cooling measures.
