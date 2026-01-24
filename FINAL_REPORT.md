## PROJECT SUMMARY
This project simulated an external reconnaissance and initial access phase of a red-team engagement against a deliberately vulnerable target. The goal was to identify exposed services, assess attack surface risk, and demonstrate realistic initial access paths in a controlled lab environment.

## Key Findings
- Multiple externally exposed legacy services were identified
- Telnet allowed direct system access using default credentials
- FTP permitted anonymous authentication and directory access
- Both services transmitted data without encryption, increasing risk

## Lesson Learned
This project reinforced the importance of service exposure management and the risks posed by legacy protocols. Even without exploiting software vulnerabilities, insecure configurations alone can lead to full system compromise.
