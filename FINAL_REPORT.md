## PROJECT SUMMARY
This project simulated an external reconnaissance and initial access phase of a red-team engagement against a deliberately vulnerable target. The objective was to identify exposed services, assess attack surface risk, and demonstrate realistic initial access paths within a controlled lab environment.

## Key Findings
- Multiple externally exposed legacy services were identified
- Telnet allowed direct system access using default credentials
- FTP permitted anonymous authentication and directory access
- Both services transmitted data without encryption, increasing risk

## Lesson Learned
This project reinforced the importance of service exposure management and the risks posed by legacy protocols. Even in the absence of software exploitation, insecure configurations alone can provide attackers with a viable path to system compromise.
