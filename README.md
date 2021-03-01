# COSE242_arp_ethernet

## Assignment 1
**1. Ethernet Packet Capture Using Wireshark**
  - Summary: Ethernet frame header analysis of ECHO(ping) request and reply(2 Frames)
  - Submission:
    1) Packet capture screenshot  
    2) Ethernet header analysis report (Ethernet Header Only)

**2. 802.11 Packet Capture Using Wireshark**
  - Summary: Understand how packets are actually generated and transmitted from the end host to the end host. (Under 802.11 environment)
  - Submission: 
    1) ICMP Packet Capture using ping program
    2) Report the analysis about IEEE 802.11 Header (IEEE 802.11 MAC, LLC, SNAP) of ICMP packets
    3) Explain the reason why the L2 (DLL) headers are presented differently on network monitor and wireshark.
    4) Packet capture screenshot (network monitor, wireshark)

**3. PPP Survey_PPP Execution Example**
  - Summary: Understand how ppp hosts negotiate options and exchange their frame between themselves.
  - Submission:
    1) Explain how ppp daemon negotiate each other, using captured ppp frame. (Refer to RFC 1661 (LCP), 1662 (HDLC-PPP)). It should include analysis of the dumped frames (pppdump output)
 ---

## Assignment 2_Implementation of Simple ARP Program
  - Summary:
    1) Learning how to use the Ethernet directly from the application layer.
    2) Understanding the Ethernet Frame, the EUI-48 MAC address, and ethernet type.
    3) Exercise the socket API of the L2 layer for the Linux operating system.
 - Program Outline:
    1) Virtual machine VM1 and VM2 is set as a wired connections. Data are sent from VM1 to VM2, and VM2 sends reply message against packet VM1 sent. (Suppose there is no VM2's prior sending)
    2) On first sending from VM1 to VM2, now knowing MAC addres of VM2, ARP should be preceded. After getting VM2's MAC address, VM1 sends data to VM2.
    3) Send additional data to from VM1 to VM2. As VM1 has recognized VM2's MAC address from prior step, it can send data without performing ARP.  
      
    ![image](https://user-images.githubusercontent.com/62787552/109516870-0930dd80-7aec-11eb-96c7-8d16999fcb8c.png)

test