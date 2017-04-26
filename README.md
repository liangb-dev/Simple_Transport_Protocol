# Simple_Transport_Protocol

This project creates a tiny TCP/IP stack and communicates with an HTTP server to retrieve a document. 

The network connection is established over a TCP scoket connection to login-faculty.ccs.neu.edu on port 5025. 

The program first sends an preemptive ARP request to the server. After receiving an ACK response to from the server, the program sends back
a packet with specific data and parameters to establish the connection. Data packets will then continously be streamed to the program 
from the server until the server closes the connection via a FIN flag. 
