# Telecommunication Signaling Protocols
Telecommunication networks use various **signaling protocols** to establish, control, and terminate calls and data sessions across different network types, from traditional landlines to modern 5G networks. The main categories include:

## Legacy TDM Protocols
These protocols were developed primarily for the Public Switched Telephone Network (PSTN), which uses time-division multiplexing (TDM) and circuit switching.

#### Signaling System No. 7 (SS7): 
An international standard that uses dedicated out-of-band signaling channels to exchange control information between network switches. It enables core services like call setup, routing, caller ID, and SMS. The SS7 protocol stack includes user parts such as the **Telephony User Part (TUP)** and the **ISDN User Part (ISUP)** for call control, and the **Mobile Application Part (MAP)** for mobile network services like roaming.
    
#### Channel Associated Signaling (CAS):
A method where signaling information (like on-hook/off-hook status) is conveyed within the same channel as the voice traffic, often using "robbed bits" in digital carriers or specific tones in analog systems.
    
#### Dual-Tone Multi-Frequency (DTMF): 
The most common form of in-band signaling used on customer premises, where dialing digits produce specific combinations of two tones (the touch-tones on a keypad).
    

## IP-Based Protocols (VoIP and Mobile Data)
As networks migrated to Internet Protocol (IP), new signaling protocols were developed to manage sessions over packet-switched networks.

#### Session Initiation Protocol (SIP): 
The dominant application-layer protocol for managing multimedia sessions (voice, video, instant messaging) over IP networks. It is a key component of the IP Multimedia Subsystem (IMS) architecture used in modern cellular networks (VoLTE, VoWiFi).
    
#### Diameter: 
A modern, IP-based protocol used in 4G and 5G networks for Authentication, Authorization, and Accounting (AAA) functions, managing subscriber access, policy control, and real-time charging. It effectively replaced legacy protocols like RADIUS in core networks.
    
#### GPRS Tunneling Protocol (GTP): 
A set of IP-based protocols that carry General Packet Radio Service (GPRS) user data and control signaling within GSM, UMTS, and LTE core networks, facilitating mobility and seamless internet connectivity.
    
#### SIGTRAN (Signaling Transport): 
A suite of protocols that enable the transport of legacy SS7 signaling over IP networks. This facilitates the convergence of traditional PSTN and modern IP infrastructures using a reliable transport layer like the Stream Control Transmission Protocol (SCTP).
    
#### Media Gateway Control Protocol (MGCP) and Megaco/H.248: 
Protocols used to control media gateways (which convert TDM voice traffic to IP packets and vice-versa) from a centralized media gateway controller.
    

**Summary of Key Protocols by Network Generation**

| Network Generation | Primary Signaling Protocols |
| -------- | ------- |
| **Legacy/PSTN** | SS7 (ISUP, TUP, MAP), CAS, DTMF, ISDN (Q.931) |
| **3G/4G**| Diameter, SIP, GTP, SIGTRAN, MAP, INAP/CAP |
| **5G**| Diameter, SIP, GTP (enhanced interfaces like N1N2, N4) |

