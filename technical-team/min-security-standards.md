---
permalink: /technical-team/min-security-standards
title: Minimum Security Standards
author:
- Epoch Technical Team
---
# Technical Team Policies - Minimum Security Standards

## §1. Definition of Terms

1.  The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
    "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this
    document are to be interpreted as described in the IETF's RFC 2119,
    excluding the changes made in RFC 8174 (both UPPERCASE and lowercase
    usage of the key words have the defined special meanings).

## §2. Authority to Enforce
Epoch Bylaws - Title 2, Chapter 1

## §3. Overview
This document is intended to outline the minimum security policies that should be implemented with Epoch sensitive data and systems. 

## §4. Waiving Policies
Any of the minimum security standard policies may be waived jointly by the Epoch Technical Team, provided that:
1. There is a supermajority vote among the leaders of the Epoch Technical Team to waive the policy.
2. There is a legitimate operational need to waive the policy.
3. There is a legitimate operational reason that the policy must be waived (there is no workaround that will fulfill operational needs). 
4. The reasons for, the voting record, and the scope of the waiver is documented.
5. The Epoch Staff Advisor and Epoch Technical Advisors are consulted before any waivers are issued, and are notified of the waiver's issuance.

## §5. Server Security Policies
The following minimum security standards must be followed on Epoch systems.

### §5.1 Low Risk Systems
* Patch all high severity vulnerabilities published in the Common Vulnerabilities and Exposures (CVE) database within seven days of publication in the database.
* Patch all other vulnerabilities published in the CVE database within ninety days of publication in the database.
* Enable host firewall in default deny mode, and only permit the neccessary minimum services. 
* Review host access and sudoer policies periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team).
* Run malware and virus scans periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team).
* Password-protect and secure iLO, IPMI, and other server management technologies.
* Enforce password complexity and password expiry requirements

### §5.2 Medium Risk Systems
All of the above policies, plus:
* Require two-factor authentication for administrator logins
* Enforce HTTPS and other encrypted channels for information transfer.
  * No information may be sent or recieved to or from a medium-risk system via an unencrypted channel, unless approved in writing by a leader of the Epoch Technical Team, or their designee.
* Secure physical hardware via locks, gates, cameras, etc.

### §5.3 High Risk Systems
All of the above policies, plus: 
* Access systems only through a bastion host.
* Confer with leaders of the Epoch Technical Team before any changes are made to the systems, or before any high-risk systems are deployed.

## §6. Application Security Policies
The following minimum security standards must be followed on Epoch applications.
### §6.1 Low Risk Applications
* Patch all high severity vulnerabilities published in the Common Vulnerabilities and Exposures (CVE) database within seven days of publication in the database.
* Patch all other vulnerabilities published in the CVE database within ninety days of publication in the database.
* Enable host firewall in default deny mode, and only permit the neccessary minimum services. 
* Review host access and sudoer policies periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team).
* Run malware and virus scans periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team
* Enforce password complexity and password expiry requirements
* Conduct security audits and review logs periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team).

### §6.2 Medium Risk Applications
All of the above policies, plus:
* Require two-factor authentication for administrator logins
* Enforce HTTPS and other encrypted channels for information transfer.
  * No information may be sent or recieved to or from a medium-risk system via an unencrypted channel, unless approved in writing by a leader of the Epoch Technical Team, or their designee.
* Include security as a design requirement on all code. Conduct security audits on all code and correct identified issues prior to deployment.
* Back up application data periodically (with a period to be determined jointly by the leaders of the Epoch Technical Team). Encrypt data in-transit and at rest.[^1]

### §6.3 High Risk Applications
All of the above policies, plus: 
* Access applications only through a bastion host.
* Confer with leaders of the Epoch Technical Team before any changes are made to the applications, or before any high-risk systems are deployed.


[^1]: Encryption must meet NIST-approved standards to protect Epoch's data. Encryption keys/passwords must be properly managed. In particular, secret cryptographic keys must not be stored or transmitted along with the data they protect. Cryptographic keys have the same classification as the most sensitive data they protect.


## Changelog

1.  Adopted: February 20, 2020
2.  Amended: February 21, 2020
