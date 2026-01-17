## Attacker VM Baseline
The Kali Linux attacker VM was successfully deployed and accessed using a standard user account. System stability and network interface availability were verified prior to any engagement activity.

## Network Isolation
The attacker VM was connected to a host-only VirtualBox network to ensure all activity remained within the authorized lab environment and could not interact with external systems.

## Target VM Deployment
An intentionally vulnerable Linux system (Metasploitable2) was deployed as the target environment. The system was connected to the same isolated host-only network as the attacker VM to simulate an external attacker discovering an exposed host within a controlled lab.

## Attacker–Target Visibility Verification
- The attacker system was assigned a private IP address within the isolated lab subnet.
- The target system was assigned a private IP address within the same isolated subnet as the attacker VM.
- Basic network visibility between the attacker and target systems was verified using a limited ICMP check. This confirmed that both systems could communicate within the authorized lab environment prior to reconnaissance activities.
