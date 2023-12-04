<h1 align="center">Capture a Packet with TCPDump</h1>

<h2 align="center">Project Description</h2>

<p align="center">You’re a network analyst who needs to use tcpdump to capture and analyze live network traffic from a Linux virtual machine.</p>

<h3 align="center">Task 1 - Identify Network Interfaces</h3>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/ac64d6b7-fb60-427d-a08d-a5503e0a8c44" alt="1a" /></p>

<p align="center">Using <code>sudo ifconfig</code> to identify the available interfaces and <code>tcpdump</code> to identify available options for packet capture.</p>

<h3 align="center">Task 2 - Inspect the Network Traffic of a Network Interface with TCPDump</h3>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/ad4d6f0b-9d5d-43b9-b651-e7f3edfa79cc" alt="2a" /></p>

<p align="center"><code>-i eth0</code> was used to capture data specifically from the eth0 interface.</p>
<p align="center"><code>-v</code> is used to display detailed packet data.</p>
<p align="center"><code>-c5</code> means to capture 5 packets of data.</p>

<h3 align="center">Task 3 - Capture Network Traffic with TCPDump</h3>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/d38fcd43-07bf-42f3-a56b-6bdabf4b96da" alt="3a" /></p>

<p align="center"><code>-nn</code> to have tcpdump not resolve IP addresses or ports to names. Considered best practice and prevents malicious actors from being alerted to an investigation.</p>
<p align="center"><code>&</code> is an instruction to the Bash shell to run the command in the background.</p>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/5292a922-6a72-462d-919a-ebb5ce8e035e" alt="3b" /></p>

<p align="center">Curl was used to open a website and generate HTTP traffic to be captured.</p>

<h3 align="center">Task 4 - Filter the Capture Packet Data</h3>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/da2fd8f5-3890-415d-b108-6cb509340847" alt="4a" /></p>

<p align="center"><code>-nn</code> to disable port and protocol name lookup.</p>
<p align="center"><code>-r</code> to read capture data from the named file.</p>
<p align="center"><code>-v</code> to display detailed packet data.</p>

<p align="center"><img src="https://github.com/GeoffreyMorren/TCPDump/assets/152500568/ffbd5834-d8e1-4728-970a-6b07d82437e2" alt="4b" /></p>

<p align="center"><code>-X</code> to display hexadecimal and ASCII output format packet data to be analyzed and detect patterns or anomalies during malware analysis or forensic analysis.</p>

<h2 align="center">Summary</h2>

<p align="center">In this assignment, I was able to learn how to identify network interfaces and use the tcpdump command to capture network data for inspection with the goal to interpret the information that tcpdump outputs regarding a packet.</p>
