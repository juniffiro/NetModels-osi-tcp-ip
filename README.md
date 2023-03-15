## 🌐 Model and Concept of OSI and TCP/IP

✍ <br/>
[Ukrainian version](ua.md) <br/>
[Russian version](ru.md)

## OSI model concept and basic protocols

The *OSI* model (Open Systems Interconnection Basic Reference Model, 1978) is an abstract
network model for communications and the development of network protocols.
Represents a layered approach to networking. Each layer serves its own part of
the interaction process. Thanks to this structure, the cooperation of network
equipment and software becomes much simpler, more transparent and clearer.

Today, the main protocol stack in use is *TCP/IP*, the development of which was not
related to the OSI model and, moreover, was carried out before its adoption.
During the entire existence of the OSI model, it has not been
implemented and, obviously, will never be implemented.
Only a subset of the OSI model is in use today.
It is believed that the model is too complex, and its
implementation will take too much time.

Some experts also claim that the history of the OSI model is a typical
example of a failed and disconnected project.

| №   | Layer        | Data type             | Function                                   | Example                                           |
|-----|--------------|-----------------------|--------------------------------------------|---------------------------------------------------|
| 7   | Application  | Message               | Access to network services                 | HTTP, FTP, SMTP, DNS, SSH                         |
| 6   | Presentation | Data                  | Representation and <br/>encryption of data | ASCII, JPEG, GIF, SSL, TLS                        |
| 5   | Session      | Data                  | Network session management                 | NetBIOS, Sockets                                  |
| 4   | Transport    | Segment<br/> Datagram | Direct connection <br/>between points      | TCP, UDP                                          |
| 3   | Network      | Packets               | Routing and logical<br/> addressing        | IPv4, IPv6, AppleTalk, Routers                    |
| 2   | Data link    | Frames                | Physical addressing <br/>(LLC, MAC)        | IEEE, Ethernet, DSL, Switches                     |
| 1   | Physical     | Bits                  | Signals, network environment               | USB, twisted pair, optical<br/> cable, coax, hubs |

## Concepts and basic protocols of the TCP/IP stack

TCP/IP is a network model for transferring data presented in digital form.
The model describes the method of data transmission from the information
source to the recipient. The model assumes the passage of information
through four levels, each of which is described by a rule (transmission protocol).
Sets of rules that solve the problem of data transfer make up the
stack of data transfer protocols on which the Internet is based.

The name TCP/IP comes from the two most important protocols of the family
*Transmission Control Protocol (TCP)* and *Internet Protocol (IP)*
The protocols were first developed and described in this standard.

| №   | Layer             | Data type             | Function                              | Example                                                                  |
|-----|-------------------|-----------------------|---------------------------------------|--------------------------------------------------------------------------|
| 4   | Application       | Message               | Access to network services            | HTTP, FTP, SMTP, DNS, SSH, Telnet                                        |
| 3   | Transport         | Segment<br/> Datagram | Direct connection <br/>between points | TCP, UDP                                                                 |
| 2   | Network           | Packets               | Routing and logical<br/> addressing   | IPv4, IPv6, IPSec, AppleTalk                                             |
| 1   | Network interface | Frames                | Signals, network environment          | Ethernet, IEEE 802.11, USB, twisted pair, optical<br/> cable, coax, hubs |
