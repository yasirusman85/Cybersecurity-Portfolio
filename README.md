### Scenario
You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 

To address this security event, the network security team implemented: 

A new firewall rule to limit the rate of incoming ICMP packets

Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets

Network monitoring software to detect abnormal traffic patterns

An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

### Report

### Summary
Our organization faced a DDoS attack this morning, disrupting system functionality for two hours. The attacker inundated the system with ICMP packets, prompting the incident management team to respond by blocking incoming ICMP, halting non-critical services, and restoring critical network functions.

### Identify
The security team conducted system audits, revealing the flood of ICMP packets as the cause for system failure.

### Protect
- Implemented a new firewall rule to limit incoming ICMP packets.
- Enforced source IP address verification on the firewall to prevent spoofed addresses.
- Deployed network monitoring software to detect abnormal traffic patterns.
- Utilized an IDS/IPS system to filter suspicious ICMP traffic.

### Detect
To enhance future detection capabilities, the team will use a firewall logging tool and an IDS to monitor all incoming internet traffic for unauthorized access.

### Respond
The incident management team promptly blocked incoming ICMP, halted non-critical services, and restored critical network functions.

### Recover
The system will be restored to full functionality after addressing the attack.
