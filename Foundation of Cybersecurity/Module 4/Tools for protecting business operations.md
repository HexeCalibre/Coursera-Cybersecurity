# Tools for protecting business operations
Previously, you were introduced to several technical skills that security analysts need to develop. You were also introduced to some tools entry-level security analysts may have in their toolkit. In this reading, you’ll learn more about how technical skills and tools help security analysts mitigate risks.

## An entry-level analyst’s toolkit
Every organization may provide a different toolkit, depending on its security needs. As a future analyst, it’s important that you are familiar with industry standard tools and can demonstrate your ability to learn how to use similar tools in a potential workplace. 

![](../img/entry-level-toolkit.png)

### Security information and event management (SIEM) tools
 A **SIEM tool** is an application that collects and analyzes log data to monitor critical activities in an organization. A **log** is a record of events that occur within an organization’s systems. Depending on the amount of data you’re working with, it could take hours or days to filter through log data on your own. SIEM tools reduce the amount of data an analyst must review by providing alerts for specific types of threats, risks, and vulnerabilities.

SIEM tools provide a series of dashboards that visually organize data into categories, allowing users to select the data they wish to analyze. Different SIEM tools have different dashboard types that display the information you have access to. 

SIEM tools also come with different hosting options, including on-premise and cloud. Organizations may choose one hosting option over another based on a security team member’s expertise. For example, because a cloud-hosted version tends to be easier to set up, use, and maintain than an on-premise version, a less experienced security team may choose this option for their organization.

### Network protocol analyzers (packet sniffers)
A **network protocol analyzer**, also known as a **packet sniffer**, is a tool designed to capture and analyze data traffic in a network. This means that the tool keeps a record of all the data that a computer within an organization's network encounters. Later in the program, you’ll have an opportunity to practice using some common network protocol analyzer (packet sniffer) tools. 

### Playbooks
A **playbook** is a manual that provides details about any operational action, such as how to respond to a security incident. Organizations usually have multiple playbooks documenting processes and procedures for their teams to follow. Playbooks vary from one organization to the next, but they all have a similar purpose: To guide analysts through a series of steps to complete specific security-related tasks. 

For example, consider the following scenario: You are working as a security analyst for an incident response firm. You are given a case involving a small medical practice that has suffered a security breach. Your job is to help with the forensic investigation and provide evidence to a cybersecurity insurance company. They will then use your investigative findings to determine whether the medical practice will receive their insurance payout. 

In this scenario, playbooks would outline the specific actions you need to take to conduct the investigation. Playbooks also help ensure that you are following proper protocols and procedures. When working on a forensic case, there are two playbooks you might follow:

- The first type of playbook you might consult is called the **chain of custody** playbook. Chain of custody is the process of documenting evidence possession and control during an incident lifecycle. As a security analyst involved in a forensic analysis, you will work with the computer data that was breached. You and the forensic team will also need to document who, what, where, and why you have the collected evidence. The evidence is your responsibility while it is in your possession. Evidence must be kept safe and tracked. Every time evidence is moved, it should be reported. This allows all parties involved to know exactly where the evidence is at all times.

- The second playbook your team might use is called the **protecting and preserving evidence** playbook. Protecting and preserving evidence is the process of properly working with fragile and volatile digital evidence. As a security analyst, understanding what fragile and volatile digital evidence is, along with why there is a procedure, is critical. As you follow this playbook, you will consult the **order of volatility**, which is a sequence outlining the order of data that must be preserved from first to last. It prioritizes volatile data, which is data that may be lost if the device in question powers off, regardless of the reason. While conducting an investigation, improper management of digital evidence can compromise and alter that evidence. When evidence is improperly managed during an investigation, it can no longer be used. For this reason, the first priority in any investigation is to properly preserve the data. You can preserve the data by making copies and conducting your investigation using those copies.

#### Key takeaways
> In this reading, you learned about a few tools a security analyst may have in their toolkit, depending on where they work. You also explored two important types of playbooks: chain of custody and protecting and preserving evidence. However, these are only two procedures that occur at the beginning of a forensic investigation. If forensic investigations interest you, you are encouraged to further explore this career path or security practice. In the process, you may learn about forensic tools that you want to add to your toolkit. While all of the forensic components that make up an investigation will not be covered in this certificate program, some forensic concepts will be discussed in later courses.

#### Resources for more information
>The Google Cybersecurity Action Team's 
[Threat Horizon Report](https://services.google.com/fh/files/blogs/gcat_threathorizons_full_sept2022.pdf) provides strategic intelligence for dealing with threats to cloud enterprise.
>
> The Cybersecurity & Infrastructure Security Agency (CISA) has a list of 
[Free Cybersecurity Services and Tools.](https://www.cisa.gov/resources-tools/resources/free-cybersecurity-services-and-tools) Review the list to learn more about open-source cybersecurity tools.

---

# Use tools to protect business operations
Previously, you were introduced to programming, operating systems, and tools commonly used by cybersecurity professionals. In this reading, you’ll learn more about programming and operating systems, as well as other tools that entry-level analysts use to help protect organizations and the people they serve. 

## Tools and their purposes

### Programming 
**Programming** is a process that can be used to create a specific set of instructions for a computer to execute tasks. Security analysts use programming languages, such as Python, to execute automation. **Automation** is the use of technology to reduce human and manual effort in performing common and repetitive tasks. Automation also helps reduce the risk of human error.

Another programming language used by analysts is called Structured Query Language (SQL). **SQL** is used to create, interact with, and request information from a database. A **database** is an organized collection of information or data. There can be millions of data points in a database. A **data point** is a specific piece of information. 

### Operating systems
An **operating system** is the interface between computer hardware and the user. Linux®, macOS®, and Windows are operating systems. They each offer different functionality and user experiences. 

Previously, you were introduced to **Linux** as an open-source operating system. Open source means that the code is available to the public and allows people to make contributions to improve the software. Linux is not a programming language; however, it does involve the use of a command line within the operating system. A **command** is an instruction telling the computer to do something. A **command-line** interface is a text-based user interface that uses commands to interact with the computer. You will learn more about Linux, including the Linux kernel and GNU, in a later course.

### Web vulnerability
A **web vulnerability** is a unique flaw in a web application that a threat actor could exploit by using malicious code or behavior, to allow unauthorized access, data theft, and malware deployment.

To stay up-to-date on the most critical risks to web applications, review the 
[Open Web Application Security Project (OWASP) Top 10.](https://owasp.org/www-project-top-ten/)

### Antivirus software
**Antivirus software** is a software program used to prevent, detect, and eliminate malware and viruses. It is also called anti-malware. Depending on the type of antivirus software, it can scan the memory of a device to find patterns that indicate the presence of malware. 

### Intrusion detection system
An **intrusion detection system** (IDS) is an application that monitors system activity and alerts on possible intrusions. The system scans and analyzes network packets, which carry small amounts of data through a network. The small amount of data makes the detection process easier for an IDS to identify potential threats to sensitive data. Other occurrences an IDS might detect can include theft and unauthorized access.

### Encryption
Encryption makes data unreadable and difficult to decode for an unauthorized user; its main goal is to ensure confidentiality of private data. **Encryption** is the process of converting data from a readable format to a cryptographically encoded format. **Cryptographic encoding** means converting plaintext into secure ciphertext. **Plaintext** is unencrypted information and **secure ciphertext** is the result of encryption.  

> **Note:** Encoding and encryption serve different purposes. Encoding uses a public conversion algorithm to enable systems that use different data representations to share information.    

### Penetration testing
**Penetration testing**, also called pen testing, is the act of participating in a simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes. It is a thorough risk assessment that can evaluate and identify external and internal threats as well as weaknesses.

#### Key takeaways
> In this reading, you learned more about programming and operating systems. You were also introduced to several new tools and processes. Every organization selects their own set of tools. Therefore, the more tools you know, the more valuable you are to an organization. Tools help security analysts complete their tasks more efficiently and effectively.