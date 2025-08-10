# Task 1

This repository contains my solutions for the analysis of two pcap files.

## File 1
**Credentials: ** Username - "test", Password - "test"

The screenshot of the wireshark analysis is given below.
<img width="1920" height="1020" alt="Screenshot 2025-08-10 110324" src="https://github.com/user-attachments/assets/763ae979-e5a5-4253-b79f-2bc3dfd9fde2" />

And the following is the details of the packet containing the plaintext credentials.
<img width="1531" height="720" alt="Screenshot 2025-08-10 110239" src="https://github.com/user-attachments/assets/b82822a0-ca46-42e1-a240-728dfd013026" />


## File 2
The given file seems to contain packets from various IP addresses to a single IP - "10.10.10.10". After applying two filters - "! ip.dst == 10.10.10.10" and "! (tcp.flags.syn == 1 && tcp.flags.ack == 0)", there were no packets following the given filters, signalling a possible SYN flood attack to "10.10.10.10" from multiple hosts. 
The screenshots are shown below.
<img width="1920" height="1020" alt="Screenshot 2025-08-10 140709" src="https://github.com/user-attachments/assets/c7bc446d-b6da-47d1-b6cd-a8c4446a78b0" />
<img width="1920" height="1020" alt="Screenshot 2025-08-10 140043" src="https://github.com/user-attachments/assets/39433ce4-9e65-4ad0-a4e7-7782a1329737" />
<img width="1920" height="1020" alt="Screenshot 2025-08-10 144034" src="https://github.com/user-attachments/assets/f04f4aa7-9c03-492f-8019-728534291859" />

