# TASK-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark.-


Wireshark Packet Capture Analysis

📋 Task Overview

This task involves using Wireshark, a popular network protocol analyzer, to capture and analyze real-time network traffic. By observing the packets, filtering by protocols, and exporting the data, we aim to identify the types of communication happening on a typical network session.

🛠 Steps to Perform

1. Download and install Wireshark from the official website:
   
        https://www.wireshark.org/download.html

    Follow the installation steps appropriate for your operating system.

    Ensure that you allow permission to capture packets on the network.


2. Start Capturing on an Active Network Interface

   Open Wireshark.

   Select your active network interface (e.g., Ethernet, Wi-Fi).

   Click on the Start Capture button (blue shark fin icon).


3. Generate Traffic

    While Wireshark is capturing:Open a web browser and navigate to any website (e.g., https://example.com).

    Alternatively, open a terminal/command prompt and use the ping command:

        ping google.com



4. Stop Capture

    Allow traffic to generate for about 1 minute.

    Click the Stop Capture button (red square icon).


5. Filter Captured Packets by Protocol

   Use Wireshark's filter bar to filter by specific protocols:

   HTTP: http

   DNS: dns

   TCP: tcp

   Apply these filters one by one to inspect packet details.


6. Identify at Least 3 Different Protocols

   Based on the capture, you should be able to identify at least three protocols such as:

   TCP (Transmission Control Protocol)

   DNS (Domain Name System)

   HTTP (Hypertext Transfer Protocol)

   Other possibilities include: ARP, HTTPS, UDP, ICMP, etc.



7. Export the Capture as a .pcap File

   Go to File > Export Specified Packets...

   Save the capture with a descriptive name, such as network_capture.pcap.



📊 Findings Summary
Example Protocols Observed:
Protocol	Purpose	Port
DNS	Resolves domain names to IP addresses	53
TCP	Handles reliable transport of data	Various
HTTP	Web traffic in plain text	80
Example Packet Details:

1. DNS Query
Source: Local IP
Destination: DNS Server (e.g., 8.8.8.8)
Info: Standard query for domain name (e.g., example.com)



2. TCP Handshake
SYN, SYN-ACK, ACK packets exchanged between client and server.



3. HTTP Request/Response
HTTP GET request sent to a web server.
HTTP 200 OK response with webpage content.

📌 Notes
Ensure you're authorized to capture network traffic on your network.
Avoid capturing sensitive or encrypted personal data.
