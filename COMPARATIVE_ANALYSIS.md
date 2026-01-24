## Analysis of Initial Access Vectors

Multiple initial access vectors were identified during the engagement. This section compares Telnet and FTP as potential entry points from an attacker’s perspective, considering effort, reliability, and potential impact.

| Factor | Telnet | FTP |
|--------|--------|-----|
| Authentication | Default credentials | Anonymous access |
| Encryption | None | None |
| Access Type | Interactive shell | File-level access |
| Initial Impact | Direct command execution | Information disclosure / staging |
| Attacker preference | High | High |

From an attacker’s perspective, Telnet provides immediate interactive access, making it an attractive first choice when default credentials are present. FTP, while often providing more limited access, requires minimal effort and may still expose sensitive information or enable staging for further compromise. In practice, an attacker may test both vectors and prioritize the one that yields the fastest and most reliable foothold.

In this scenario, Telnet represents the higher-risk initial access vector due to the combination of unencrypted communication and direct system interaction. FTP remains a significant supporting vector that could facilitate reconnaissance or secondary access.
