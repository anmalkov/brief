**Principle:** Confidentiality and Integrity  
**Affected Asset:** Inbound Internet connections  
**Threat:** As a result of the vulnerability of not encrypting data, plaintext data could be intercepted during transit via a man-in-the-middle (MitM), downgrade or cross-protocol attacks attack. Sensitive data could be exposed or tampered to allow further exploits.

**Mitigation:**

All products and services must encrypt data in transit using approved cryptographic protocols and algorithms.

1. Use TLS to encrypt all HTTP-based network traffic. Use other mechanisms, such as IPSec, to encrypt non-HTTP network traffic that contains customer or confidential data.
2. Use only TLS 1.2 or TLS 1.3. Use ECDHE-based ciphers suites and NIST curves. Use strong keys. Enable HTTP Strict Transport Security (HSTS). Turn off TLS compression and do not use ticket-based session resumption.