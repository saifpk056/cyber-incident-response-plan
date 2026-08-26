# 🛡️ MITRE ATT&CK Mapping

## 1. Purpose

This document maps behaviors from the fictional ransomware tabletop exercise to relevant **MITRE ATT&CK Enterprise techniques**.

The mapping is used for defensive training and incident-response planning.

It does not indicate that these techniques were actually observed in a real Internee.pk incident.

---

## 2. Technique Mapping

| ATT&CK ID | Technique | Exercise Scenario | Defensive Response |
|---|---|---|---|
| T1566 | Phishing | A fictional phishing email is used as a possible initial-access scenario. | Email filtering, security awareness training, MFA |
| T1486 | Data Encrypted for Impact | Files become inaccessible in the ransomware simulation. | Isolation, backups, recovery procedures |
| T1490 | Inhibit System Recovery | The exercise considers possible attempts to affect recovery resources. | Protected and tested backups |
| T1083 | File and Directory Discovery | An attacker may identify files and directories before impact. | Endpoint monitoring and least privilege |
| T1135 | Network Share Discovery | The scenario considers discovery of shared network resources. | Network segmentation and monitoring |
| T1570 | Lateral Tool Transfer | The exercise considers possible movement of tools between systems. | Endpoint and network monitoring |
| T1531 | Account Access Removal | The scenario considers possible disruption of account access. | Account monitoring and account recovery procedures |

---

# 3. T1566 — Phishing

### Description

Phishing can be used as an initial-access method in which a user is targeted through a malicious or deceptive message.

### Scenario

A fictional employee receives a suspicious email containing an unexpected attachment or link.

### Defensive Measures

- Security awareness training
- Email filtering
- Attachment scanning
- Link protection
- Multi-factor authentication
- User reporting procedures

---

# 4. T1486 — Data Encrypted for Impact

### Description

Data may be encrypted by an attacker to disrupt access to information.

### Scenario

During the tabletop exercise, several fictional project files become inaccessible.

### Defensive Measures

- Endpoint monitoring
- Network monitoring
- Secure backups
- Backup testing
- Rapid system isolation
- Recovery procedures

---

# 5. T1490 — Inhibit System Recovery

### Description

An attacker may attempt to prevent an organization from recovering affected systems.

### Scenario

The exercise considers the possibility that recovery resources could be targeted.

### Defensive Measures

- Maintain protected backups
- Keep backup copies separated from production systems
- Regularly test restoration
- Restrict backup administration
- Monitor backup infrastructure

---

# 6. T1083 — File and Directory Discovery

### Description

Attackers may attempt to identify files and directories on compromised systems.

### Scenario

The exercise considers possible discovery of important project files before the simulated impact.

### Defensive Measures

- Least-privilege access
- Endpoint monitoring
- File-access logging
- Unusual activity detection

---

# 7. T1135 — Network Share Discovery

### Description

Attackers may attempt to identify shared network resources.

### Scenario

The exercise considers whether shared storage could be affected.

### Defensive Measures

- Network segmentation
- Access control
- Network monitoring
- Restrict unnecessary shared resources

---

# 8. T1570 — Lateral Tool Transfer

### Description

Tools or files may be transferred between compromised systems during an attack.

### Scenario

The tabletop exercise considers possible movement between systems.

### Defensive Measures

- Endpoint monitoring
- Network monitoring
- Application allowlisting
- Restrict unnecessary administrative access

---

# 9. T1531 — Account Access Removal

### Description

An attacker may attempt to disrupt access to accounts.

### Scenario

The exercise considers possible disruption of employee account access.

### Defensive Measures

- Multi-factor authentication
- Account monitoring
- Strong password policies
- Privileged access management
- Account recovery procedures

---

# 10. Defensive Response Summary

The MITRE ATT&CK mapping supports the following defensive priorities:

1. Detect suspicious activity quickly.
2. Protect user accounts.
3. Isolate affected systems.
4. Protect backup infrastructure.
5. Monitor network activity.
6. Preserve evidence.
7. Recover from verified clean backups.
8. Train employees to recognize suspicious activity.
9. Review incidents and improve security controls.

---

# 11. Important Note

MITRE ATT&CK is a framework for describing adversary tactics and techniques.

The techniques in this document are used to support a **fictional educational ransomware exercise**.

They should not be interpreted as evidence of an actual attack against Internee.pk.

---

# 🔗 References

- MITRE ATT&CK Enterprise: https://attack.mitre.org/matrices/enterprise/
- MITRE INC Ransomware: https://attack.mitre.org/software/S1139/
- MITRE BlackByte 2.0: https://attack.mitre.org/software/S1181/
- MITRE LockerGoga: https://attack.mitre.org/software/S0372/
- CISA Ransomware Guide: https://www.cisa.gov/stopransomware/ransomware-guide

---

## 🎯 Final Defensive Workflow

**Detect → Analyze → Contain → Eradicate → Recover → Learn**
