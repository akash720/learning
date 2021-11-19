# OSI Model

#### Application layer: 
 - producing data and serves as window for apps like browser to access network and display information
 - protocols: http smtp ftp telnet

#### Presentation layer: 
- translation, data compression, encryption
- protocols: ssl(secure socket layer)

#### Session layer: 
- session management, authentication and authorization
- protocols: NetBIOS (network basic i/p o/p system)

#### Transport layer: 
- segmentation, flow and error control, 
- protocols: 
    - TCP(connection oriented, slower as feedback present, lost data can be recovered)
    - UDP(connectionless, faster as no feedback, lost data cannot be transmitted)

#### Network layer: 
- logical addressing(assigning ip address to sender and receiver), path determining, routing
- protocols: IPv4, IPv6

#### Data Link layer: 
- controls how data is placed and received from the media (media access control), error detection
- protocols: Point to point protocol(PPP), Address Resolution protocol(ARP)

#### Physical layer: 
- responsible for the actual physical connection between the devices, synchronization, convert data to binary data bits
- protocols: DSL, USB
