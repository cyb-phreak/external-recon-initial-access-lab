## Reconnaissance Methodology
Reconnaissance was performed from an attacker's perspective to identify exposed network services that could contribute to initial access. Scanning was intentionally limited in scope and intensity to reduce noise and reflect realistic attacker behavior.

## Target Identification
The target system was identified within the isolated lab network and assigned a private IP address. A minimal ICMP check confirmed that the target host was reachable within the lab environment.

## Service Discovery Result Summary

| Port | Service | Observation |
|-----|---------|------------|
| 21  | FTP     | Exposed to network |
| 22  | SSH     | Remote access enabled |
| 23  | Telnet  | Legacy remote access |
| 80  | HTTP    | Web service available |
| 3306 | MySQL  | Exposed database service |

Note: A full Nmap scan was performed, but results were summarized here to highlight services most relevant to initial access. Raw scan output is omitted for clarity.

From an attacker’s perspective, exposed services increase the attack surface and may indicate misconfigurations or outdated software that could enable an initial foothold.


## Attack Surface Analysis
Attack surface analysis was performed to prioritize exposed services based on their likelihood of leading to initial access. Factors considered included service exposure, common misconfigurations, and historical abuse by attackers.

### FTP (Port 21)
FTP is a common initial access vector due to frequent misconfigurations such as anonymous access, weak credentials, or outdated software. It often has backdoors that give immediate root access.

### HTTP (Port 80)
Web services are high-value targets because they are externally accessible and frequently interact with user input. An attacker would assess the web application for outdated software, default content, or exposed administrative interfaces.

### Telnet (Port 23)
Telnet provides remote command-line access without encryption and is considered insecure by modern standards. These are high-value targets due to frequent association with weak authentication practices and legacy system configurations.

Based on the analysis, FTP and Telnet were identified as the most likely candidates for initial access due to their exposure and historical abuse. Further reconnaissance will focus on validating whether these services present exploitable conditions.
