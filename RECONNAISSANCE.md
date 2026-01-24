## Reconnaissance Methodology
Reconnaissance was performed from an attacker's perspective to identify exposed network services that could contribute to initial access. Scanning was intentionally limited in scope and intensity to reduce noise and reflect realistic attacker behavior.

## Target Identification
The target system was identified within the isolated lab network and assigned a private IP address. A minimal ICMP check confirmed that the target host was reachable within the lab environment.

## Service Discovery Result Summary

| Port | Service | Observation |
|------|---------|------------|
| 21   | FTP     | Exposed to network |
| 22   | SSH     | Remote access enabled |
| 80   | HTTP    | Web service available |
Note: A full Nmap scan was performed, but results were summarized here to highlight services most relevant to initial access. Raw scan output is omitted for clarity.

From an attacker’s perspective, exposed services increase the attack surface and may indicate misconfigurations or outdated software that could enable an initial foothold.
