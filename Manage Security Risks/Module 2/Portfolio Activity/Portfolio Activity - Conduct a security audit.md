### Botium Toys: Scope, Goals, and Risk Assessment Report

#### Scope and Goals of the Audit
**Scope:** The scope of this audit is defined as the entire security program at Botium Toys. This includes their assets like employee equipment and devices, their internal network, and their systems. You will need to review the assets Botium Toys has and the controls and compliance practices they have in place.

**Goals:** Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices that need to be implemented to improve Botium Toys’ security posture.

#### Current Assets
Assets managed by the IT Department include:
- On-premises equipment for in-office business needs
- Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
- Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
- Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
- Internet access
- Internal network
- Data retention and storage
- Legacy system maintenance: end-of-life systems that require human monitoring

#### Risk Assessment
**Risk Description:** Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards.

**Control Best Practices:** The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

**Risk Score:** On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

**Additional Comments:** The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:
- Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.
- Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database.
- Access controls pertaining to least privilege and separation of duties have not been implemented.
- The IT department has ensured availability and integrated controls to ensure data integrity.
- The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
- Antivirus software is installed and monitored regularly by the IT department.
- The IT department has not installed an intrusion detection system (IDS).
- There are no disaster recovery plans currently in place, and the company does not have backups of critical data.
- The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
- Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters).
- There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
- While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
- The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.

### Controls Assessment Checklist

| Yes/No | Control | Explanation |
| --- | --- | --- |
| No | Least Privilege | All employees currently have access to customer data; access should be restricted to minimize breach risks. |
| No | Disaster recovery plans | There are no existing disaster recovery plans, which are essential for ensuring business continuity in case of disruptions. |
| No | Password policies | The current password policies are weak, making it easier for threat actors to access sensitive data through employee devices and the network. |
| No | Separation of duties | Separation of duties is needed to reduce fraud risk and prevent unauthorized access to critical data, as the CEO handles daily operations and payroll. |
| Yes | Firewall | The firewall is configured with security rules that effectively manage and block traffic. |
| No | Intrusion detection system | An IDS is required to detect potential intrusions by malicious actors. |
| No | Backups | Critical data backups are necessary to maintain business continuity in the event of a breach. |
| Yes | Antivirus software | Antivirus software is installed and regularly monitored by the IT department. |
| No | Manual monitoring, maintenance, and intervention for legacy systems | Legacy systems are monitored and maintained, but without a regular schedule or clear procedures, they remain at risk. |
| No | Encryption | Encryption is not used, which would enhance the confidentiality of sensitive information. |
| No | Password Management System | A password management system is needed to improve productivity and manage password issues effectively. |
| Yes | Locks (offices, storefront, warehouse) | The physical location has adequate locks for security. |
| Yes | Closed-circuit television (CCTV) surveillance | CCTV surveillance is operational at the physical location. |
| Yes | Fire detection/prevention (Fire alarm, sprinkler system, etc.) | The physical location is equipped with a functioning fire detection and prevention system. |

### Compliance Checklist

| Yes/No | Best Practice | Explanation |
| --- | --- | --- |
| No | Only authorized users have access to customers' credit card information | All employees currently have access to internal data, including customer credit card information. |
| No | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. | Credit card data is not encrypted, and all employees can access this sensitive information. |
| No | Implement data encryption procedures to better secure credit card transaction touchpoints and data | Encryption is not implemented, which is necessary to ensure the confidentiality of customer financial data. |
| No | Adopt secure password management policies | Current password policies are inadequate, and a password management system is needed. |

### GDPR Checklist

| Yes/No | Best Practice | Explanation |
| --- | --- | --- |
| No | E.U. customer's data is kept private/secured. | Encryption is needed to protect the privacy of E.U. customers' financial information. |
| Yes | There is a plan in place to notify E.U customers within 72 hours if their data is compromised/there is a breach | A notification plan is in place to inform E.U. customers within 72 hours of a data breach. |
| No | Ensure data is properly classified and inventoried | Assets are inventoried but not classified, which is necessary for better data management. |
| Yes | Enforce privacy policies, procedures, and processes to properly document and maintain data. | Privacy policies, procedures, and processes are enforced among IT staff and other employees as required. |

### SOC Type 1, Type 2 Checklist

| Yes/No | Best Practice | Explanation |
| --- | --- | --- |
| No | User access policies are established. | Least privilege and separation of duties are not enforced, so all employees have access to internal data. |
| No | Sensitive data PII/SPII is confidential/private | Encryption is needed to ensure the confidentiality of sensitive personal information. |
| Yes | Data integrity ensures the data is consistent, complete, accurate, and has been validated | Data integrity measures are in place. |
| No | Data is available to individuals authorized to access it. | Access to data should be limited to authorized personnel only. |

### Recommendations

Based on the risk assessment and current state of controls and compliance, the following recommendations are made to improve Botium Toys’ security posture and compliance:

1. **Implement Least Privilege and Separation of Duties:**
   - Restrict access to sensitive data, ensuring only authorized personnel have access.
   - Implement separation of duties to reduce the risk of internal fraud and errors.

2. **Develop Disaster Recovery Plans:**
   - Establish and document disaster recovery plans to ensure business continuity in the event of an incident.
   - Regularly test and update these plans to address evolving risks.

3. **Enhance Password Management:**
   - Adopt a centralized password management system that enforces strong password policies.
   - Ensure password policies meet current security standards, including complexity and rotation requirements.

4. **Deploy an Intrusion Detection System (IDS):**
   - Implement IDS to detect and respond to potential security breaches in real-time.

5. **Regular Backups:**
   - Establish a regular backup schedule for critical data and systems.
   - Ensure backups are stored securely and tested for integrity and availability.

6. **Implement Encryption:**
   - Encrypt sensitive data, including customers' credit card information, both in transit and at rest.
   - Ensure encryption protocols meet industry standards and are regularly reviewed and updated.

7. **Compliance with PCI-DSS and GDPR:**
   - Ensure compliance with PCI-DSS by securing credit card processing and storage environments.
   - Implement data classification and inventory practices to maintain GDPR compliance, ensuring all personal data is properly documented and protected.

8. **User Access Policies:**
   - Develop and enforce user access policies to control access to sensitive information.
   - Regularly review and update these policies to address changing business needs and emerging threats.

By addressing these areas, Botium Toys can significantly reduce its risk profile, enhance its security posture, and ensure compliance with relevant regulations.
