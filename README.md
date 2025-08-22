 # Project Summary

## This project simulated a Security Operations Center (SOC) for BazTech Inc. to demonstrate how segmentation, log monitoring, and incident response can defend against cyber        threats. Using pfSense, the network was segmented into WAN, LAN, IT Department, and DMZ. Security tools like Wazuh Manager and Wazuh Agents where installed. A red-team           simulation with Kali Linux executed a brute-force SSH attack on the DMZ server, exposing segmentation weaknesses and enabling lateral movement.

# Key Achievements
## . Designed a segmented network using pfSense with WAN, LAN, IT, and DMZ.
## . Deployed Wazuh Manager and Wazuh agents for threat visibility.
## . Successfully simulated a brute-force SSH attack and captured logs.
## . Detected lateral movement from LAN ➝ DMZ through SIEM alerts.
## . Validated the importance of firewall rule enforcement in segmentation.

# Findings.
## . Brute-force Detection: Multiple failed logins flagged before successful credential compromise.
## . Segmentation Bypass: Firewall rules allowed unrestricted SSH from LAN to DMZ.
## . Lateral Movement Risk: Compromise of DMZ host created pivoting opportunities deeper into the network.

# Recommendations.
## . Restrict SSH access to DMZ only from a secure Management VLAN (jump box).
## . Block all LAN-to-DMZ traffic by default, allowing only web services (HTTP/HTTPS).
## . Apply Zero Trust principles with strict ACLs.
## . Continuously monitor logs and alerts via SIEM for brute-force/lateral movement attempts.

# Impacts.
## . Demonstrated how weak segmentation enables attackers to bypass defenses.
## . Showed that unrestricted management protocols (SSH) create single-hop compromise risks.
## . Validated SOC’s role in detecting, containing, and mitigating real-world attack scenarios.
## . Highlighted the need for firewall precision + layered security controls to protect enterprise network.

## See belowe for the full report.
[Report]


