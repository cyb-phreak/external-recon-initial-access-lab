## Telnet Initial Access Validation
Initial access validation was performed to determine whether the exposed Telnet service presents a realistic authentication attack surface. Actions were intentionally limited to avoid unauthorized access beyond validating exposure.

### Telnet Exposure Assessment
A connection to the Telnet service was successfully established, and an interactive login prompt was presented. This confirms that the service is accessible from the network and accepts authentication attempts over an unencrypted channel.

Based on this validation, the Telnet service was confirmed to present a realistic initial access vector. Further authentication testing could be justified in a controlled engagement scenario.

## Initial Access Demonstration
This section demonstrates how an attacker could obtain an initial foothold via an exposed Telnet service using known default credentials in a controlled lab environment. The demonstration is intentionally limited to initial access only.

### Result
Authentication to the Telnet service was successful using documented default credentials. This confirms that an attacker could gain an initial foothold on the system without exploiting a software vulnerability.

### Impact Assessment
Successful access via Telnet provides interactive command-line access to the system. From this position, an attacker could potentially enumerate the system, access sensitive files, or attempt lateral movement.

### Why This Worked
This issue exists due to the use of an insecure legacy protocol combined with default credentials. Telnet transmits authentication data in cleartext and provides no protection against credential interception.

### Recommended Remediation
- Disable Telnet and replace with SSH
- Enforce strong, unique credentials
- Restrict remote management services using network controls
- Monitor authentication attempts on remote access services
