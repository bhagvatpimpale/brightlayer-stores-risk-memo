# brightlayer-stores-risk-memo
MEMORANDUM
TO: BrightLayer Stores Management
FROM: Junior Security Analyst
DATE: October 5, 2026
SUBJECT: Cybersecurity Risk Assessment & Mitigation Recommendations
1. FIVE IMPORTANT ASSETS
 * Employee Email Accounts: Critical for daily communications, internal coordination, vendor contacts, and sensitive business correspondence.
 * Shared Computers: Physical hardware used by staff to perform daily store operations, access business tools, and interface with corporate data.
 * Company Website: Primary public face for customer engagement, marketing, and online brand presence.
 * Cloud Storage (Invoices & User Passwords): Houses essential financial records, vendor transaction histories, and stored credentials vital for operational continuity.
 * Public Wi-Fi Router: Enables internet connectivity for both store operations and visiting customers.
2. THREE POTENTIAL THREATS
 * Threat 1 (External Cybercriminals / Phishers): Cybercriminals launching targeted phishing attacks to trick employees into handing over login credentials or executing malware.
 * Threat 2 (Unauthenticated Public Users / Malicious Guests): Individuals connected to the public Wi-Fi network attempting to intercept unencrypted traffic or scan internal devices.
 * Threat 3 (Untrusted Internal / External Threat Actors): Opportunistic attackers attempting to brute-force or intercept weak, plain-text, or reused passwords stored in cloud storage.
3. THREE VULNERABILITIES
 * Vulnerability 1 (Lack of Network Segmentation): The public Wi-Fi router does not isolate guest users from internal store networks or shared office hardware.
 * Vulnerability 2 (Insecure Credential Storage & Access Controls): Storing user passwords in accessible cloud files without proper encryption or Multi-Factor Authentication (MFA) controls.
 * Vulnerability 3 (Shared User Accounts & Human Factors): Multiple employees sharing physical computers without individual login accounts or security awareness training.
4. ASSOCIATED RISKS
 * Risk 1 (Threat 1 + Vulnerability 3): Compromise of Shared Devices & Email Accounts.
   * Impact: A phishing email opened on a shared computer compromises credentials, leading to unauthorized access, operational disruption, and potential business data theft.
 * Risk 2 (Threat 2 + Vulnerability 1): Public Wi-Fi Traffic Eavesdropping & Network Intrusion.
   * Impact: Malicious actors on the public Wi-Fi intercept store data or pivot to shared computers on the same network, causing data exposure and loss of network integrity.
 * Risk 3 (Threat 3 + Vulnerability 2): Unauthorized Cloud Data & Financial Record Breach.
   * Impact: Attackers gain unauthorized access to stored invoices and customer/user passwords, leading to financial loss, legal penalties, and severe reputational damage.
 * Risk 4 (Threat 1 + Vulnerability 2): Ransomware or Credential Harvesting via Cloud Storage.
   * Impact: Attackers use stolen cloud credentials to encrypt or alter critical invoices, halting business operations and causing financial loss.
 * Risk 5 (Threat 2 + Vulnerability 3): Unauthorized Physical & Logical Access to Shared Hardware.
   * Impact: An untrusted individual accesses an unattended shared computer, exposing company emails and internal systems, resulting in local data loss or tampering.
5. SECURITY RECOMMENDATIONS
 * Implement Network Segmentation (Mapped to Risk 2): Configure a dedicated, isolated Guest VLAN on the Wi-Fi router to separate customer traffic completely from internal store systems and shared computers.
 * Deploy Multi-Factor Authentication & Enforce Password Management (Mapped to Risk 3): Mandatory MFA across cloud storage and email logins; migrate plain-text user passwords out of cloud documents into a secure enterprise password manager.
 * Establish Unique User Accounts & Screen Lock Policies (Mapped to Risk 5): Assign distinct employee logins on all shared computers and enforce an automated 5-minute screen lock policy.
 * Deploy Endpoint Protection & Conduct Phishing Awareness Training (Mapped to Risk 1): Install EDR/Antivirus on all shared workstations and train employees to recognize credential-harvesting emails.
 * Encrypt Stored Invoices & Implement Access Controls (Mapped to Risk 4): Apply Role-Based Access Control (RBAC) and end-to-end encryption to cloud storage containing invoices, restricting access solely to authorized personnel.
