# OSI Model 

Explain the 7 layers of the OSI model with a practical example using SMTP protocol.



The Open Systems Interconnection (OSI) model is a **reference model**developed by the International Organization for Standardization (ISO) that "provides a common basis for the coordination of standards development for the purpose of systems interconnection.

The **TCP/IP** Model is what is widely used in practical networking and forms the foundation of the internet.

For the actual specifications, we can view the RFC's: 

- [RFC 1122](https://www.rfc-editor.org/rfc/rfc1122)
- [RFC 1123](https://www.rfc-editor.org/rfc/rfc1123)

These documents give a structured specification for implementation.


## The seven layers of the OSI model

| S.No | Layer | Role | Example |
| ---  | ---   | ---- | ---               |
| 7    | Application Layer | interacts directly with the user data, think of it as an interface for the applications to use. | HTTP,FTP,SMTP,SSH |
| 6    | Presentation Layer | makes the data presentable for the application layer, responsible for translation,encryption or compression | TLS | 
| 5    | Session Layer | opening, maintaing and closing communication between the two devices. It synchornizes the data transfer and keeps the connection alive | TCP |
| 4    | Transport Layer | responsible for end-to-end communication. This includes taking data from the session layer and breaking it up into chunks called segments before sending it to layer 3. | TCP | 
| 3    | Network Layer   | facilitates data transfer between two different networks, breaks up segments into smaller units called packets. Finds the best physical path(routing) | IP,ICMP | 
| 2    | Data Link layer | physical addressing on the local network segment, finding where to deliver the data | MAC addresses, ethernet frames | 
| 1    | Physical Layer  | The physical medium/connection between the devices such as cables and switches | | 


