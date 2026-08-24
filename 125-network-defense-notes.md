# Network Defense Notes

## Module 1: Understanding Defense

### 1.1 Defense-in-Depth
#### 1.1.1 Assets, Vulnerabilities, Threats

As a cybersecurity analyst, it is my job to secure the assets of the organization's network.

- **Assets** - Anything of value to an organization that must be protected including servers, infrastructure devices, end devices, and the greatest asset, data.
- **Vulnerabilities** - A weakness in a system or its design that could be exploited by a threat actor.
- **Threats** - Any potential danger to an asset

#### 1.1.2 Identify Assets

As an organization grows, so do its assets. Consider the number of assets a large organization would have to protect. It may also acquire other assets through mergers with other companies. The result is that many organizations only have a general idea of the assets that need to be protected.

The collection of all the devices and information owned or managed by the organization are assets. The assets constitute the attack surface that threat actors could target. These assets must be inventoried and assessed for the level of protection needed to thwart potential attacks.

Asset management consists of inventorying all assets, and then developing and implementing policies and procedures to protect them. This task can be daunting considering many organizations must protect internal users and resources, mobile workers, and cloud-based and virtual services.

Further, organizations need to identify where critical information assets are stored, and how access is gained to that information. Information assets vary, as do the threats against them. For example, a retail business may store customer credit card information. An engineering firm will store competition-sensitive designs and software. A bank will store customer data, account information, and other sensitive financial information. Each of these assets can attract different threat actors who have different skill levels and motivations.

#### 1.1.3 Asset Classification

Asset classification assigns an organization's resources into groups based on common characteristics.

The most critical information needs to receive the highest level of protection and may even require special handling.

A labeling system can be used to determine how valuable, how sensitive, and how critical the information is.

##### Step 1:

Determine the proper asset identification category:

- Information assets
- Software assets
- Physical assets
- Services

##### Step 2

Establish asset accountability by identifying the owner of each information asset and each piece of software:

- Identify the owner for all information assets
- Identify the owner for all application software

##### Step 3

Determine the criteria for classification

- Confidentiality
- Value
- Time
- Access rights
- Destruction

##### Step 4

Implement a classification scheme:

Adopt a consistent way of identifying information to ensure uniform protection and easier monitoring

Asset standards identify specific hardware and software products used by an organization.

When a failure occurs, prompt action helps to maintain both access and security. If an organization does not standardize its hardware selection, personnel may need to scramble to find a replacement component. Non-standard environments require more expertise to manage, and they increase the cost of maintenance contracts and inventory.

#### 1.1.6 Asset Lifecycle Stages

For cybersecurity specialists, part of the job is to manage information assets and related systems throughout that asset's lifecycle

##### Procurement

The organization purchases the assets based on the needs identified from the data gathered to justify the purchase

The asset is added to the organization's inventory

##### Deployment

The asset is assembled and inspected to check for defects or other problems. Staff perform tests and install tags or barcodes for tracking purposes

The asset moves from inventory to in-use

##### Utilization

This is the longest stage of the cycle. The asset's performance is continuously checked. Upgrades, patch fixes, new license purchases and compliance audits are all part of the utilization stage

##### Maintenance

Maintenance helps to extend an asset's productive life. Staff may modify or upgrade the asset

##### Disposal

At the end of the asset's productive life, it must be disposed of. All data must be wiped from the asset. Disposal may include dismantling an asset for parts. Any parts that can cause an environmental hazard must be disposed of according to local guidelines

#### 1.1.8 Identify Vulnerabilities

##### Identified e-banking Threats

Threat identification provides an organization with a list of likely threats for a particular environment. When identifying threats, it is important to ask several questions

- What are the possible vulnerabilities of a system?
- Who may want to exploit those vulnerabilities to access specific information assets?
- What are the consequences if system vulnerabilities are exploited and assets are lost?

The threat identification for an e-banking system would include:

- **Internal system compromise** - The attacker uses the exposed e-banking servers to break into an internal bank system
- **Stolen customer data** - An attacker steals the personal and financial data of bank customers from the customer database
- **Phony transactions from an external server** - An attacker alters the code of the e-banking application and makes transactions by impersonating a legitimate user
- **Phony transactions using a stolen customer PIN or smart card** - An attacker steals the identity of a customer and completes malicious transactions from the compromised account
- **Insider attack on a system** - A bank employee finds a flaw in the system from which to mount an attack
- **Data input errors** - A user inputs incorrect data or makes incorrect transaction requests
- **Data center destruction** - A cataclysmic event severely damages or destroys the data center

Identifying vulnerabilities on a network requires an understanding of the important applications that are used, as well as the different vulnerabilities of that application and hardware. This can require a significant amount of research on the part of the network administrator

#### 1.1.9 Identify Threats

##### Defense-in-Depth Approach

Organizations must use a defense-in-depth approach to identify threats and secure vulnerable assets. This approach uses multiple layers of security at the network edge, within the network, and on network endpoints.

- **Edge router** - The first line of defense is known as an edge router. The edge router has a set of rules specifying which traffic it allows or denies. It passes all connections that are intended for the internal LAN to the firewall
- **Firewall** - The second line of defense is the firewall. The firewall is a checkpoint device that performs additional filtering and tracks the state of the connections. It denies the initiation of connections from the outside (untrusted) network to the inside (trusted) network while enabling internal users to establish two-way connections to the untrusted networks. It can also perform user authentication (authentication proxy) to grant external remote users access to internal network resources
- **Internal router** - Another line of defense is the internal router. It can apply final filtering rules on the traffic before it is forwarded to its destination

Other security devices used in a defense-in-depth approach are:

- **Intrusion Prevention Systems (IPS)**
- **Advanced Malware Protection (AMP)**
- **Web and Email content security systems**
- **Identity Services**
- **Network Access Controls**

In the layered defense-in-depth security approach, the different layers work together to create a security architecture in which the failure of one safeguard does not affect the effectiveness of the other safeguards

#### 1.1.10 The Security Onion and the Security Artichoke

##### Security Onion

A common analogy in which a threat actor would have to peel away at a network's defenses layer by layer in a manner similar to peeling an onion. Only after penetrating each layer would the threat actor reach the target data or system 

##### Security Artichoke

The changing landscape of networking, such as the evolution of borderless networks, has changed this analogy to the “security artichoke”, which benefits the threat actor.

As illustrated in the figure, threat actors no longer have to peel away each layer. They only need to remove certain “artichoke leaves.” The bonus is that each “leaf” of the network may reveal sensitive data that is not well secured.

For example, it’s easier for a threat actor to compromise a mobile device than it is to compromise an internal computer or server that is protected by layers of defense. Each mobile device is a leaf. And leaf after leaf, it all leads the hacker to more data. The heart of the artichoke is where the most confidential data is found. Each leaf provides a layer of protection while simultaneously providing a path to attack.

Not every leaf needs to be removed in order to get at the heart of the artichoke. The hacker chips away at the security armor along the perimeter to get to the “heart” of the enterprise.

While internet-facing systems are usually very well protected and boundary protections are typically solid, persistent hackers, aided by a mix of skill and luck, do eventually find a gap in that hard-core exterior through which they can enter and go where they please.

#### 1.1.11 Defense in Depth Strategies

##### Layering

To make sure data and information remains available, an organization must set up different layers of protection, creating a barrier of multiple defenses that work together to prevent attacks. A good example of layering is an organization storing its top-secret documents on a password-protected server in a locked building that is surrounded by an electric fence.

A layered approach provides the most comprehensive protection because, even if cybercriminals penetrate one layer, they still must contend with several more defenses. Ideally, each layer should be more complicated to overcome!

Defense in depth does not provide an impenetrable shield, but it will help an organization minimize risk by staying one step ahead of cybercriminals.

##### Limiting

Limiting access to data and information reduces the possibility of a security threat. An organization should restrict access so that each user only has the level of access required to do their job.

An organization should have the right tools and settings, such as file permissions, in place to limit access, as well as the right procedural measures, which define specific steps for doing anything that can affect security. For example, a limiting procedure which requires employees to always consult sensitive documents in a room which has CCTV, ensures that they would never remove such documents from the premises.

##### Diversity

If all defense layers were the same, it would not be very difficult for cybercriminals to succeed in an attack. The layers must be different so that if one layer is penetrated, the same technique will not work on all the others which would compromise the whole system. Furthermore, an organization will normally use different encryption algorithms and authentication systems to protect data in different states.

To accomplish the goal of diversity in defenses, organizations can use security products by different companies as different factors of authentication, such as a swipe card from one company and a fingerprint reader manufactured by a different company — as well as varied security measures, such as time-delay locks on cabinets and supervision by a security staff member upon unlocking it.

##### Obscurity

Obscuring information can also protect data and information. An organization should not reveal any information that cybercriminals can use to identify which Operating System (OS) a server is running, or the type or make of equipment or software it uses.

Error messages or system information should not contain any details that a cybercriminal could use to determine what vulnerabilities are present. Concealing certain types of information makes it more difficult for cybercriminals to attack.

##### Simplicity

Complexity does not necessarily guarantee security. If an organization implements complex systems that are hard to understand and troubleshoot, this may backfire. If employees do not understand how to configure a solution properly, such as setting up their account using an unnecessarily complex process, this may make it just as easy for cybercriminals to compromise those systems.

A security solution should be simple from the inside, but complex on the outside.

### 1.2 Cybersecurity Operations Management
#### 1.2.2 Configuration Management

Configuration management refers to identifying, controlling and auditing the implementation and any changes made to a system’s established baseline.

The baseline configuration includes all the settings that you configure for a system which provide the foundation for all similar systems — like a template of sorts.

For instance, those responsible for deploying Windows workstations to users must install the required applications and set up the system settings according to a documented configuration. This is the baseline configuration for Windows workstations within this organization.

Documented configuration resources might inlude the following:

- Network maps, cabling and wiring diagrams, application configuration specification
- Standards naming conventions used for computers
- IP schema to track IP addresses

Hardening the operating system is an important part of making sure that systems have secure configurations. Configuring log files along with auditing, changing default account names and passwords, implementing account policies and file-level access control are all used to create a secure OS

#### 1.2.3 Log Files

A log records all events as they occur. Log entries make up a log file, with each log entry containing all the information related to a specific event. Accurate and complete logs are very important in cybersecurity.

For example, an audit log tracks user authentication attempts, while an access log records details on requests for specific files on a system. Monitoring system logs will therefore help us determine how an attack occurred and which of the defenses deployed were successful — and which were not.

As an increasing number of log files are generated for computer security purposes, organizations should consider a log management process. Management of computer security log data should determine the procedures for the following:

- Generating log files
- Transmitting log files
- Storing log files
- Analyzing log data
- Disposing of log data

#### 1.2.4 Operating System Logs and Application Security Logs

##### Operating System Logs

Operating system logs record events that are linked to actions that have to do with the operating system. System events include the following:

- Client requests and server responses such as succesful user authentications
- Usage information that contains the number and size of transactions in a given period of time

##### Application Security Logs

Organizations use network-based and/or system-based security software to detect malicious activity

This software generates a security log to provide computer security data. These logs are useful for performing auditing analysis and identifying trends and long-term problems. Logs also enable an organization to provide documentation showing that it complies with laws and regulatory requirements

#### 1.2.5 Protocol Analyzers

Packet analyzers, otherwise known as packet sniffers, intercept and log network traffic.

The packet analyzer captures each packet, looks at the values of various fields in the packet and analyzes its content. It can capture network traffic on both wired and wireless networks.

Packet analyzers perform the following functions:

- Traffic logging
- Network problem analysis
- Detection of network misuse
- Detection of network intrusion attempts
- Isolation of exploited systems

### 1.3 Security Policies, Regulations, and Standards
#### 1.3.1 Business Policies

Business policies are the guidelines that are developed by an organization to govern its actions. The policies define standards of correct behavior for the business and its employees. In networking, policies define the activities that are allowed on the network. This sets a baseline of acceptable use. If behavior that violates business policy is detected on the network, it is possible that a security breach has occurred

An organization. may have several guiding policies:

##### Company policies 

- These policies establish the rules of conduct and the responsibilities of both employees and employers. 
- Policies protect the rights of workers as well as the business interests of employers
- Depending on the needs of the organization, various policies and procedures establish rules regarding employee conduct, attendance, dress code, privacy and other areas related to the terms and conditions of employment

##### Employee Policies

- These policies are created and maintained by human resources staff to identify employee salary, pay schedule, employee benefits, work schedule, vacations, and more
- They are often provided to new employees to review and sign

##### Security Policies

- These policies identify a set of security objectives for a company, define the rules of behavior for users and administrators, and specify system requirements
- These objectives, rules, and requirements collectively ensure the security of a network and the computer systems in an organization
- Much like a continuity plan, a security policy is a constantly evolving document based on changes in the threat landscape, vulnerabilities, and business and employee requirements

#### 1.3.2 Security Policy

A comprehensive security policy has a number of benefits, including the following:

- Demonstrates an organization's commitment to security
- Sets the rules for expected behavior
- Ensures consistency in system operations, software and hardware acquisition and use, and maintenance
- Defines the legal consequences of violations
- Gives security staff the backing of management

Security policies are used to inform users, staff, and managers of an organization's requirements for protecting technology and information assets. A security policy also specifies the mechanisms that are needed to meet security requirements and provides a baseline from which to acquire, configure, and audit computer systems and networks for compliance

The table lists policies that may be included in a security policy.

| Policy | Description |
| --- | --- |
| Identification and authentication policy | Specifies authorized persons that can have access to network resources and identity verification procedures |
| Password policies | Ensures passwords meet minimum requirements and are changed regularly |
| Acceptable Use Policy (AUP) | Identifies network applications and uses that are acceptable to the organization. It may also identify ramifications if this policy is violated |
| Remote Access Policy | Specifies network device operating systems and end user application update procedures |
Network maintenance policy | Specifies network device operating systems and end user application update procedures |
| Incident handling procedures | Describes how security incidents are handled |

One of the most common security policy components is an AUP. This can also be referred to as an appropriate use policy. This component defines what users are allowed and not allowed to do on the various system components. This includes the type of traffic that is allowed on the network. The AUP should be as explicit as possible to avoid misunderstanding

#### 1.3.3 BYOD Policies

Many organizations must now also support Bring Your Own Device (BYOD). This enables employees to use their own mobile devices to access company systems, software, networks, or information. BYOD provides several key benefits to enterprises, including increased productivity, reduced IT and operating costs, better mobility for employees, and greater appeal when it comes to hiring and retaining employees.

However, these benefits also bring an increased information security risk because BYOD can lead to data breaches and greater liability for the organization

A BYOD security policy should be developed to accomplish the following:

- Specify the goals of the BYOD program
- Identify which employees can bring their own devices
- Identify which devices will be supported
- Identify the level of access employees are granted when using personal devices
- Describe the rights to access and activities permitted to security personnel on the device
- Identify which regulations must be adhered to when using employee devices
- Identify safeguard to put in place if a device is compromised

This table lists BYOD security best practices to help mitigate BYOD vulnerabilities

| Best Practice | Description |
| --- | --- |
| Password protected access | Use unique passwords for each device and account | 
| Manually control wireless connectivity | Turn off Wi-Fi and Bluetooth connectivity when not in use. Connect only to trusted networks |
| Keep updated | Always keep the device OS and other software updated. Updated software often contains security patches to mitigate against the latest threats or exploits | 
| Back up data | Enable backup of the device in case it is lost or stolen |
| Enable "Find my Device | Subscribe to a device locator service with remote wipe feature |
| Provide antivirus software | Provide antivirus software for approved BYOD devices |
| Use Mobile Device Management (MDM) software | MDM software enables IT teams to implement security settings and software configurations on all devices that connect to company networks |

#### Regulatory and Standard Compliance

There are also external regulations regarding network security. Network security professionals must be familiar with the laws and codes of ethics that are binding on Information Systems Security (INFOSEC) professionals.

Many organizations are mandated to develop and implement security policies. Compliance regulations define what organizations are responsible for providing and the liability if they fail to comply. The compliance regulations that an organization is obligated to follow depend on the type of organization and the data that the organization handles. Specific compliance regulations will be discussed later in the course.

## Module 2: System and Network Defense

### 2.1 Physical Security

#### 2.1.2 Fencing and Physical Barriers

Fencing and barriers are the outermost later of defense and the most visible.

##### Physical Barriers

Physical barriers may have the following components:

- Perimeter fence system
- Security gate system
- Bollards (short posts used to stop vehicle intrusions)
- Vehicle entry barriers
- Guard shelters
- Fencing

##### Fencing

A fence is a barrier that encloses secure areas and designates boundaries. When designing a perimeter fencing system, the following height guidelines apply:

- 1 meter (3-4 ft) will only deter casual trespassers
- 2 meters (6-7 ft) are too high to climb by casual trespassers
- 2.5 meters (8 ft) will offer limited delay to a determined intruder

High-security areas often require a 'top guard' such as barbed wire or concertina wire. Top guards act as an additional deterrent and can delay the intruder by causing severe injury. However, attackers can still use a blanket or mattress to alleviate this threat.

Local regulations may restrict the type of fencing system an organization can use and it's important to remember that fences require regular maintenance. Animals may burrow under the fence or the earth may wash out, leaving the fence unstable — this would lead to easy access for an intruder. Fencing systems should be inspected regularly. 

Moreover, vehicles should never be parked near a security fence, as this could assist the intruder in climbing over or causing damage to the fence

#### 2.1.3 Biometrics

Biometrics are the physiological or behavioral characteristics of an individual, and there are security practices based on identifying and granting access using biometrics.

The first error rate is **Type I errors or false rejections**. A Type I error rejects a person that registers and is an authorized user. In access control, where the main objective is to keep cybercriminals away, false rejection is the least important error. It means that someone who should gain access is not granted access.

However, in many biometric applications, particularly retail or banking, false rejections can have a very negative impact on business due to a transaction or sale being lost.

False acceptance is a Type II error. **Type II errors allow entry to people who should not have entry**, meaning a cybercriminal can potentially gain access. For this reason, Type II errors are normally considered **the most important error** for a biometric access control system.

The acceptance rate is also an important concept here. Stated as a percentage, it is the rate at which a system accepts unenrolled individuals or imposters as authentic users – so the rate of Type II errors per total instances of granting permission.

#### 2.1.4 Badges and Access Logs

An access badge allows an individual to gain access to an area with automated entry points. 

#### 2.1.5 Surveillance

Many physical access controls, including deterrent and detection systems, ultimately rely on people to intervene and stop the actual attack or intrusion

##### Video and Electronic Surveillance

Video and electronic surveillance can supplement or, in some cases, replace security guards. The benefits of video and electronic surveillance include the ability to monitor areas when no other persons are present, the ability to record and log surveillance videos and data for long periods, plus being able to link to motion detection technology and notifications where appropriate.

In a highly secure environment, video and electronic surveillance should be placed at all entrances, exits, loading bays, stairwells and refuse collection areas.

##### Guards and Escorts

Security guards are a great solution for access control requiring an instantaneous and appropriate response. However, there are numerous disadvantages to using security guards, including cost and the inability to monitor and record high volumes of traffic. The use of guards also introduces the risk of human error.

In highly secure information system facilities, guards control access to the organization’s sensitive areas. The benefit of using guards here is that they can adapt more than automated systems. Guards can learn and distinguish many different conditions and situations, and make decisions on the spot.

##### RFID and Wireless Surveillance

Managing and locating important information system assets is a key challenge for most organizations. Growth in the number of mobile and IoT devices has made this job even more difficult. Time spent searching for critical equipment can lead to expensive delays or downtime. The use of Radio Frequency Identification (RFID) asset tags can be of great value to the security staff. An organization can place RFID readers in the door frames of secure areas so that they are not visible to individuals.

The benefit of RFID asset tags is that they can track any asset that physically leaves a secure area. New RFID asset tag systems can read multiple tags simultaneously. RFID systems do not require line-of-sight to scan tags, either. Another advantage of RFID is the ability to read tags that are not visible. Unlike barcodes and human-readable tags that must be physically located and openly displayed to read, RFID tags do not need to be visible to scan.

### 2.2 Application Security

#### 2.2.2 Application Development

To maintain security at all stages of application development, a robust process needs to be followed

##### Developing and testing

Software is developed and updated in a development environment, where it can be developed, tested and debugged before being deployed. A development environment is less restrictive than the live environment and has a lower security level. Version control software helps track and manage changes to the software code. Developers may also work in a sandbox environment so that code is not overwritten as they develop it. 

During testing, developers look at how the code interacts with the normal environment. Quality assurance (QA) can find defects in the software. It is much easier to fix any defect found at this phase.

##### Staging and production

Staging environments should closely match the organization’s production environment.

By testing in a staging environment, developers can verify that the software runs under the required security settings. After the developer runs and tests security, the program can be deployed to production.

##### Provisioning and deprovisioning

Provisioning is the creation or updating of software. Deprovisioning is its removal.

An organization can use a self-service portal to automate software provisioning and deprovisioning.

#### 2.2.3 Security Coding Techniques 

When coding applications, developers use several techniques to validate that all security requirements have been met.

##### Normalization

Normalization is used to organize data in a database and help maintain data integrity. Normalization converts an input string to its simplest known form to ensure that all string have unique binary representations and that any malicious input is identifies

##### Stored Procedure

A stored procedure is a group of precompiled SQL statements stored in a database that execute a task. If you use a stored procedure to accept input parameters from clients using different input data, you will reduce network traffic and get faster results.

##### Obfuscation and Camouflage

A developer can use obfuscation and camouflage to prevent software from being reverse engineered. Obfuscation hides original data with random characters or data. Camouflage replaces sensitive data with realistic fictional data.

##### Code resuse

Code reuse means using existing software to build new software, saving time and development costs. Care must be taken, though, to avoid the introduction of vulnerabilities.

##### SDKs

Third-party libraries and software development kits (SDKs) provide a repository of useful code to make application development faster and cheaper. The downside is that any vulnerabilities in SDKs or third-party libraries can potentially affect many applications.

#### 2.2.5 Input Validation

Controlling the data input process is key to maintaining database integrity. Many attacks run against a database and insert malformed data. Such attacks can confuse, crash or make the application divulge too much information to the attacker. Scroll down to look at an example — in this case, an automated input attack.

Customers fill out a web application form to subscribe to a newsletter. A database application automatically generates and sends email confirmations back to the customers. When customers receive the email with a URL link to confirm their subscription, attackers have modified the URL link. 

These modifications can change the username, email address or subscription status of the customers when they click to confirm their subscription. This way, when the email is returned to the host server, it receives bogus information, which it might not be aware of if it does not check each email address against subscription information.

Hackers can automate this attack to flood the web application with thousands of invalid subscribers to the newsletter database.

#### 2.2.6 Validation Rules

A validation rule checks that data falls within the parameters defined by the database designer. A validation rule helps to ensure the completeness, accuracy and consistency of data. The criteria used in a validation rule include the following:

- Size – checks the number of characters in a data item
- Format – checks that the data conforms to a specified format
- Consistency – checks for the consistency of codes in related data items
- Range – checks that data lies within a minimum and maximum value
- Check digit – provides for an extra calculation to generate a check digit for error detection

#### 2.2.7 Integrity Checks

Compromised data can threaten the security of your devices and systems.

**An integrity check** can measure the consistency of data in a file, picture or record to ensure that it has not been corrupted. 
The integrity check performs a **hash function** to take a snapshot of data and then uses this snapshot to ensure data has remained unchanged. 
**A checksum** is an example of a hash function.

##### How a checksum works

A checksum verifies the integrity of files, or strings of characters, before and after they transfer between devices across a local network or the Internet. Checksums convert each piece of information to a value and sum the total. To test the data integrity, a receiving system repeats the process. If the two sums are equal, the data is valid. If not, a change has occurred somewhere along the line.

##### Hash functions

Common hash functions include MD5, SHA-1, SHA-256 and SHA-512. These use complex mathematical algorithms to compare data to a hashed value. For example, after downloading a file, the user can verify the integrity of the file by comparing the hash values from the source with the ones generated by any hash calculator.

##### Version control

Organizations use version control to prevent authorized users from making accidental changes. Version control means that two users cannot update the same object, such as a file, database record or transaction, at the exact same time. For example, the first user to open a document has the permission to change that document; the second person who tries to open it while the first user is still working on it will only be able to access a read-only version.

##### Backups

Accurate backups help to maintain data integrity if data becomes corrupted. An organization needs to verify its backup process to ensure the integrity of the backup.

##### Authorization

Authorization determines who has access to an organization’s resources based on a need-to-know basis. For example, file permissions and user access controls ensure that only certain users can modify data. An administrator can set permissions for a file to read-only. As a result, a user accessing that file cannot make any changes.

#### 2.2.8 Other Application Security Practices

##### Code Signing

Code signing helps prove that a piece of software is authentic

Executables designed to install and run on a device are digitally signed to validate the author's identity and provide assurance that the software code has not changed since it was signed

##### Secure cookies

Using secure cookies protects information stored in cookies from hackers

When your client system interacts with a server, the server sends an HTTP response that instructs your browser to create at least one cookie. The cookie then stores data for future requests while you are browsing that website

#### 2.2.10 Managing Threats to Applications

Organizations can implement various measures to manage threats to the application domain

##### Unauthorized access to data centers, computer rooms, and wiring closets

- Implement policies, standards and procedures for staff and visitors to ensure the facilities are secure.

##### Server and system downtime

- Develop a business continuity plan for critical applications to maintain availability of operations.
- Develop a disaster recovery plan for critical applications and data.

##### Network operating system software vulnerability

- Develop a policy to address application software and operating system updates.
- Install patches and updates regularly.

##### Unauthorized access to systems

- Use MFA
- Monitor log files

##### Data loss

- Implement data classification standards.
- Implement backup procedures.

##### Software development vulnerabilities

- Conduct software testing prior to launch.

### 2.3 Network Hardening: Services and Protocols

#### 2.3.2 Network and Routing Services

Cybercriminals use vulnerable network services to attack a device or to use it as part of an attack. To check for insecure network services, use a port scanner to detect open ports on a device. A port scanner sends a message to each port and waits for a response, which indicates how the port is used and whether it is open.

But beware, cybercriminals also use port scanners for this same reason! Securing network services ensures that only necessary ports are exposed and available.

##### Dynamic Host Configuration Protocol (DHCP)

DHCP uses a server to assign an IP address and other configuration information to network devices. In effect, the device gets a permission slip from the DHCP server to use the network. Attackers can target DHCP servers to deny access to devices on the network, but security measures like DHCP snooping prevent rogue DHCP servers from providing IP addresses to clients by validating messages from sources that are not trusted.

A security checklist for DHCP:

- Physically secure the DHCP server.
- Apply any software patches.
- Locate the DHCP server behind a firewall.
- Monitor DHCP activity by reviewing DHCP logs.
- Maintain a strong antivirus solution.
- Uninstall any unused services and applications.
- Close unused ports.

##### Domain Name System (DNS)

DNS translates a URL or website address, such as www.cisco.com, into a numerical IP address. When users type a web address into the address bar, the DNS server will recognize the IP address. Attackers can target DNS servers to deny access to network resources or redirect traffic to rogue websites. Use secure service and authentication between DNS servers to protect them from these attacks.

DNS Security Extensions (DNSSEC) uses digital signatures to strengthen authentication and protect against threats to the DNS.

A security checklist for DNS:

- Keep DNS software up to date.
- Prevent version string from revealing information.
- Separate internal and external DNS servers.
- Restrict allowed transactions by client IP address.
- Use transaction signatures to authenticate transactions.
- Disable or restrict zone transfers and dynamic updates as much as possible.
- Enable logging and analyze logs.
- Use Domain Name System Security Extensions (DNSSEC).
- Sign zones.

##### Internet Control Messaging Protocol (ICMP)

Network devices use ICMP to send error messages, that a requested service is not available or the host could not reach the router, for example.

The ping command is a network utility that uses ICMP to test the reachability of a host on a network. Ping sends ICMP messages to the host and waits for a reply. Cybercriminals can alter the use of ICMP to run reconnaissance, denial of service (DoS) and covert channel attacks. Many networks filter ICMP requests to prevent such attacks.

##### Routing Information Protocol (RIP)

RIP is a routing protocol that limits the number of hops from source to destination that are allowed in a network path. The maximum number of hops allowed for RIP is fifteen. RIP is used to exchange routing information about which networks each router can reach and how far away those networks are.

RIP calculates the best route based on hop count, but cybercriminals can also target routers and the RIP protocol. Such attacks on routing services can affect performance and availability, some attacks can even result in traffic redirection. Use secure services with authentication and implement system patching and updates to protect routing services.

##### Network Time Protocol (NTP)

Having the correct time within networks is important. Correct timestamps accurately track network events such as security violations. Additionally, clock synchronization is critical for the correct interpretation of events within syslog data files as well as for digital certificates.

Network Time Protocol (NTP) is a protocol that synchronizes network computer system clocks. NTP allows network devices to synchronize their time settings with an NTP server. Cybercriminals attack timeservers to disrupt secure communication that depends on digital certificates and to hide attack information. Use NTP Authentication to verify that the server is trusted.

#### 2.3.3 Telnet, SSH, and SCP

##### Secure Shell (SSH)

Is a protocol that provides a secure (encrypted) remote connection to a device. Telnet is an older protocol that uses unsecure plaintext when authenticating a device (user name and password) and transmitting data. SSH should be used rather than Telnet to manage connections, as it provides strong encryption. SSH uses TCP port 22. Telnet uses TCP port 23.

##### Secure Copy (SCP)

Securely transfers files between two remote systems. SCP uses SSH for data transfer and authentication, ensuring the authenticity and confidentiality of the data in transit.

##### Wireshark Telnet capture

Cybercriminals monitor packets using Wireshark

##### Plaintext username and password capture

Cybercriminals capture the username and password of the administrator from the plaintext Telnet session

##### Wireshark SSH capture

The Wireshark view of an SSH session. Cybercriminals track the session using the IP address of the administrator device

##### Username and password encrypted

The session encrypts the username and password

#### 2.3.4 Secure Protocols

Attackers can penetrate a network’s infrastructure through services, protocols and open ports. Older protocols leave a network in a vulnerable position, so cybersecurity professionals need to make sure current protocols are being used.

##### Simple Network Management Protocol (SNMP)

SNMP collects statistics from TCP/IP devices to monitor network and computer equipment. SNMPv3 is the current standard — it uses cryptography to prevent eavesdropping and make sure data hasn’t been tampered with while in transit.

##### HTTP 

Hypertext Transfer Protocol (HTTP) provides basic web connectivity and uses port 80. HTTP contains limited built-in security and is open to traffic monitoring when transmitting content, leaving the user’s computer open to attack. 

Let’s see how other protocols provide a more secure connection:

- Secure Sockets Layer (SSL) manages encryption by using an SSL handshake at the beginning of a session to provide confidentiality and prevent eavesdropping and tampering.
- Transport Layer Security (TLS) is an updated, more secure replacement for SSL.
- SSL/TLS encrypts communication between the client and the server. Where it’s used, the user will see HTTPS in the URL field of a browser instead of HTTP.

##### FTP

File Transfer Protocol (FTP) transfers computer files between a client and a server. In FTP, the client uses a plaintext username and password to connect. File Transfer Protocol Secure (FTPS) is more secure — it adds support for TLS and SSL to prevent eavesdropping, tampering and forgery on exchanged messages.

##### POP, IMAP, MIME

Email uses Post Office Protocol (POP), Internet Message Access Protocol (IMAP) and Multipurpose Internet Mail Extensions (MIME) to attach non-text data, such as an image or video, to an email message.

To secure POP (port 110) or IMAP (port 143), use SSL/TLS to encrypt mail during transmission. The Secure/Multipurpose Internet Mail Extensions (S/MIME) protocol provides a secure method of transmission. It sends digitally signed and encrypted messages that provide authentication, message integrity and nonrepudiation.

### 2.4 Network Hardening: Segmentation

#### 2.4.2 Virtual Local Area Networks (VLANs)

Implementing a VLAN to segment the network and create a secure area for the sensitive data

- Devices are grouped

VLANs provide a way to group devices within a local area network (LAN) and on individual switches. VLANs are not the same as LANs: virtual LANs are based on logical connections, while LANs are based on physical connections. Individual ports on a switch can be assigned to a specific VLAN. Other ports can be used to physically interconnect switches and allow multiple VLAN traffic between switches. These ports are called trunks.

- The network is segmented

VLANs allow an administrator to segment a network based on factors such as function, project team or application. Devices within a VLAN act as if they are in their own independent network, even though they share a common infrastructure with other VLANs on the same LAN. A VLAN can separate groups of devices that host sensitive data from the rest of the network, decreasing the chances of confidential information breaches — in our example, the HR department looking to protect sensitive data. Trunks allow individuals on the HR VLAN to be physically connected to multiple switches.

- Data is protected

VLANs provide a way to limit broadcast traffic in a switched network. But beware, cybercriminals can attack VLAN performance and availability. To protect the VLAN, monitor its performance, use advanced configurations and regularly install patches and updates.

#### 2.4.3 The Demilitarized Zone (DMZ)

A demilitarized zone (DMZ) is a small network between a trusted private network and the Internet.

##### Access to untrusted networks

Web servers and mail servers are usually placed within the DMZ to allow users to access an untrusted network, such as the Internet, without compromising the internal network.

##### Zones of risk

Most networks have two to four zones of risk: the trusted private LAN, the DMZ, the Internet and an extranet.

- Within the LAN zone, the risk level is low, and the trust level is high.
- Within the extranet zone, the risk level is medium-low, and the trust level medium-high.
- Within the DMZ, the risk level is medium-high, and the trust level is medium-low.
- Within the Internet zone, the risk level is high, and the trust level is low. 

##### Zero Trust model

Firewalls manage east-west traffic (traffic that goes between servers within the organization’s data center) and north-south traffic (data moving into and out of the organization’s network).

To protect its network, an organization can implement a Zero Trust model. Automatically trusting users and endpoints within the organization can put any network at risk, as trusted users can move throughout the network to access data. Zero Trust networking constantly monitors all users on the network regardless of their status or role.

#### 2.4.4 Managing Threats to the LAN

- Unauthorized LAN access: Secure wiring closets, data centers and computer rooms. Deny access to anyone without the proper credentials.
- Unauthorized access to systems, applications and data: Define strict access control policies, standards, procedures and guidelines.
- Network operating system software vulnerabilities: Implement policy to patch and update operating systems.
- Unauthorized access by rogue users: Require passphrases or authentication for wireless networks.
- Exploits of data in transit: Implement encryption between devices and wireless networks.
- Unauthorized network probing and port scanning: Conduct post-configuration penetration tests.

### 2.5 Hardening Wireless and Mobile Devices

#### 2.5.2 Wireless Device Security

Wired Equivalent Privacy (WEP) was the first security protocol used for wireless networks. This was replaced by Wi-Fi Protected Access (WPA), which improved the security of wireless connections.

##### WPA Configuration

Wi-Fi Protected Access (WPA) was the computer industry’s response to the weaknesses of the WEP standard. WPA-PSK (Pre-Shared Key) is the most common WPA configuration. The keys used by WPA are 256-bit, a significant increase over the 64-bit and 128-bit keys used in the WEP system.

##### WPA features

The WPA standard provided several security improvements. First, WPA provided message integrity checks (MIC), which could detect if an attacker had captured and altered data passed between the wireless access point and a wireless client. Another key security enhancement was Temporal Key Integrity Protocol (TKIP). The TKIP standard helped to better handle, protect and change encryption keys. Advanced Encryption Standard (AES) superseded TKIP, for even better key management and encryption protection.

##### WPA2 (Wi-Fi Protected Access II)

The Wi-Fi Protected Access II (WPA2) standard was released in 2006. This introduced the mandatory use of AES algorithms and replaced TKIP with the Counter Cipher Mode with Block Chaining Message Authentication Code Protocol (CCMP).

##### WPA3 (Wi-Fi Protected Access III)

WPA3 added more features to WPA2 such as maintaining strong cryptographic algorithms and improving key exchange.

##### Wi-Fi Protected Setup (WPS)

Wi-Fi Protected Setup (WPS) can be used to set up a secure wireless home network. A PIN code is used to connect devices to the wireless network. However, WPS poses a major security vulnerability, as the user’s PIN can be discovered through brute-force attack. Due to this, WPS should not be used and should be disabled altogether.

#### 2.5.5 Authentication

Wireless devices have become predominant on most modern networks. They provide mobility and convenience but are vulnerable to a range of cybersecurity issues. They are open to theft, hacking and unauthorized remote access, sniffing, man-in-the-middle attacks, as well as attacks against performance and availability.

The best way to secure a wireless network is to use authentication and encryption. The original wireless standard, 801.11, introduced two types of authentication.

##### Open System Authentication

Any wireless device can connect to the wireless network. Use this method in situations where security is of no concern

##### Shared Key Authentication

Provides mechanisms to authenticate and encrypt data between a wireless client and AP or wireless router

#### 2.5.6 Authentication Protocols

The Extensible Authentication Protocol (EAP) is an authentication framework used in wireless networks. Let’s find out how it works.

1. The user requests to connect to the wireless network through an access point.
2. The access point requests identification data (username) from the user, which is then sent to an authentication server.
3. The authentication server requests proof that the ID is valid.
4. The access point requests proof that the ID is valid from the user, in the form of a password.
5. The user supplies the access point with their password. The access point sends this back to the authentication server.
6. The server confirms the username and password are correct, and passes this information on to the access point and user.
7. The user connects to the wireless network.

##### EAP-TLS

Requires Client Certificate: Yes
Requires Server Certificate: Yes
Easily Deployed: Difficult
Security: High

##### PEAP

Requires Client Certificate: No
Requires Server Certificate: Yes
Easily Deployed: Moderate
Security: Medium

##### EAP-TTLS

Requires Client Certificate: No
Requires Server Certificate: Yes
Easily Deployed: Moderate
Security: Medium

##### EAP-FAST

Requires Client Certificate: No
Requires Server Certificate: No
Easily Deployed: Easy
Security: Medium

#### 2.5.8 Mutual Authentication

Your wireless network and its sensitive data are susceptible to unauthorized access by hackers using a wireless connection. But what can you do to prevent an attack?

##### Rogue Access Points

An access point is any hardware device that enables other wireless devices to connect to a wired network. Any device that has a wireless transmitter and hardwired interface to a network can potentially act as a rogue or unauthorized access point.

The rogue access point will often imitate an authorized access point, allowing users to connect to the wireless network but potentially stealing their data or conducting other nefarious activity in the process. 

##### Preventing Attacks

When you connect to a rogue access point, the imposter who set it up can request and copy data from your device. This type of man-in-the-middle attack is very difficult to detect and can result in stolen login details and data.

Mutual authentication is two-way authentication that can prevent rogue access points. It is a process in which both entities in a communications link authenticate each other before they connect. This enables clients to detect rogue access points and prevent such MitM attacks. 

#### 2.5.10 Communication Methods

##### Wi-Fi and Bluetooth

Mobile devices can use wireless signals such as Wi-Fi and Bluetooth. You can configure wireless access through the device's settings menu. Bluetooth is commonly used to connect headphones or to pair a phone with a car sound system

##### Near-field Communication (NFC)

Allows contactless communication between devices. NFC chips use electromagnetic fields to enable contactless payments, meaning, for instance, that you simply need to hold your device close to a payment terminal to process a payment

##### Infrared (IR)

Provides short-range communication using an IR receiver. For example, IR allows you to control your television through your cell phone.

##### USB Communication

The only type of communication on this list that is wired, USB communication allows you to use your smartphone for data or audio storage. USB connectivity also allows a mobile device to function as a modem or fax. You can connect a mobile device to forensic acquisition devices via the USB port if you need to gather information for an investigation. 

#### 2.5.11 Mobile Device Management

A mobile device issued by an organization can contain both personal and organizational data — it can be either corporate-owned or corporate-owned personally enabled (COPE).

An organization may also have a bring-your-own-device (BYOD) option. Security and data protection policies need to be applied when there is sensitive corporate information on a user’s device.

##### Storage segmentation and containerization

Storage segmentation and containerization allow you to separate personal and work content on a device. It provides an authenticated, encrypted area that separates sensitive company information from the user’s personal data.

Containerization also enables us to:

- Isolate apps.
- Control app functions.
- Delete container information.
- Remotely wipe the device.

##### Content Management

An organization needs to consider the security risks involved in using applications that share data — for example, Dropbox, Box, Google Drive and iCloud. An identity-management security system can be used to control what data a user can access.

##### Application Management

Whitelisting allows you to digitally sign applications so that you can authorize which applications users can install. This helps to ensure that installed applications come from a trusted source.

Authentication using strong passwords is a best practice for those applications that require user credentials.

#### 2.5.12 Mobile Device Protections

Whether a mobile device is owned by the organization or is a personal device used for work, measures need to be put in place to keep it safe from cyber threats.

##### What are the risks?

Threats to mobile devices include:

- Theft
- Loss
- Unauthorized Access
- Operating system risks
- Application risks
- Network risks

##### Jailbreaking, rooting, and sideloading

Jailbreaking, rooting and sideloading are ways of bypassing a device’s limitations to do things that the device is restricted from doing. Users may try to jailbreak (Apple devices) or root (Android devices) their device to run an app that is not authorized or available in the store.

Jailbreaking removes the restriction that only Apple-authorized apps may run on the device. Rooting bypasses Android’s security architecture to allow complete, administrative access to the device. Both pose a risk to the organization. 

Solutions are available that can detect a jailbroken or rooted device. A device is then marked as noncompliant and removed from the network or denied access to organizational apps.

Third-party app stores can also pose a risk for organizations because the apps they provide access to have not been evaluated properly. Sideloading occurs when the user goes around the approved app settings to install unapproved apps. This is less invasive than jailbreaking or rooting, but it is still a risk.

##### What are the safeguards?

Safeguards against mobile device threats include the following:

- Screen locks require a password, PIN or pattern to access the device.
- Biometric authentication uses a unique physical characteristic (fingerprint, face, iris or voice).
- Context-aware authentication uses machine learning to determine access based on a user’s normal behavior.
- Remote wiping deletes the device’s data should the device be stolen or lost.
- Full device encryption can encrypt all data on a mobile device.

#### 2.5.13 GPS Tracking

Global Positioning System (GPS) uses satellites and computers to determine the location of a device. GPS technology is a standard feature on smartphones and provides real-time position tracking that can typically pinpoint a location to within approximately 5 meters.

Many cell phone apps use GPS tracking to track the phone’s location. For example, Facebook allows users to check in to a location, which is then visible to people in their networks. Some apps use geofencing or geolocation, which use radio-frequency identification (RFID) to determine a geographic area instead.

Push notifications sometimes use geolocation and geofencing too. This enables local organizations to ‘push’ advertising messages based on a user’s location settings. Unfortunately, increasingly savvy cyber attackers have started using push notifications to capture data.

#### 2.5.14 Bring Your Own Device

In order to prevent unauthorized access, devices must be password protected using the features of the device.
A strong password is required to access the network.
Employees can automatically download, install and use any app that appears on the list of approved apps.
Smartphones and tablets that are not on the list of supported devices are not allowed to connect to the network.
Employees’ access to company data is limited based on user profiles defined by IT and automatically enforced.
The organization can use remote wiping to delete the device’s data should the device be stolen or lost.

### 2.6 Cybersecurity Resilience

#### 2.6.2 High Availability

The term ‘high availability’ describes systems designed to avoid downtime as much as possible. The continuous availability of information systems is imperative, not only to organizations but to modern life, as we are all using and relying on computer and information systems more than ever before.

High availability systems typically are based on three design principles.

##### Eliminating Single Points of Failure

The first principle that defines high availability systems starts with identifying all system devices and components whose failure would result in system-wide failure. Methods to eliminate single points of failure include replacing or removing hot stand-by devices, redundant components and multiple connections or pathways.

##### Providing for Reliable Crossover

Redundant power supplies, backup power systems and backup communications systems all provide for reliable crossover — the second design principle.

##### Detecting Failures as They Occur

The third principle is active device and system monitoring to detect many types of events including system and device failures. Monitoring systems may even trigger the backup system in the case of failure.

##### 2.6.3 The Five Nines

Every organization wants to be able to operate uninterrupted, even under extreme conditions, such as during an attack.

One of the most popular high availability goals is often called ‘five nines.’ It gets its name from its aim to achieve an availability rate of 99.999%, which is five nines in a row. In practice, this means that downtime is less than 5.26 minutes per year.

##### Standardized Systems

Systems standardization provides for systems that use the same components. As a result, parts inventories are easier to maintain and it is possible and easy to swap components, even during an emergency.

In highly secure information system facilities, guards control access to the organization’s sensitive areas. The benefit of using guards here is that they can adapt more than automated systems. Guards can learn and distinguish many different conditions and situations, and make decisions on the spot.

##### Clustering 

Multiple devices grouped together provide a service that, to users, appears to be a single entity. If one device in a cluster fails, the other devices remain available and can step in

##### Shared Component Systems

Systems are built so that a complete system can stand in for one that failed

#### 2.6.4 Single Points of Failure

Single points of failure are weak links in the chain that can cause disruption of the organization's operations. A single point of failure is any part of the operation of the organization whose failure means complete failure of the entire system — in other words, if it fails, the entire system fails.   

A single point of failure can be a specific piece of hardware, a process, a specific piece of data, or even an essential utility. Generally, the solution to a single point of failure is to modify the critical operation so that it does not rely on any single element. The organization can also build redundant components into the operation to take over the process should one of these points fail.

#### 2.6.6 N+1 Redundancy

N+1 redundancy helps ensure system availability in the event of a component failure. It means that components (N) need to have at least one backup component (+1).

A good way to think about this is that a car has four tires (N) and a spare tire (+1) in the trunk in case of a flat.

Although a system using N+1 architecture contains redundant equipment, it is not a fully redundant system.

In a network, N+1 redundancy means that the system design can withstand the loss of one of each component

The N refers to each different infrastructure component that is part of the system. For example, a data center includes servers, power supplies, switches and routers. The +1 is the additional component or system that is standing by, ready when needed. N+1 redundancy in a data center that consists of the above elements means that we have a server, a power supply, a switch and a router on standby, ready to come online if something happens to the main server, the main power source, switch or router

#### 2.6.7 RAID

RAID Level Comparison

| Raid Level | Min # of Drive | Description | Advantages | Disadvantages |
| --- | --- | --- | --- | --- |
| 0 | 2 | Data stripping without redundancy | Highest performance | No data protection, failure of one drive results in all loss of all data |
| 1 | 2 | Disk mirroring | Highest performance, high data protection because all data is duplicated | High cost of implementation because an additional drive of equal or larger capacity is required |
| 2 | 2 | Error-Correcting Coding | This level is no longer used | Same performance can be achieved at a lower cost using RAID 3 |
| 3 | 3 | Byte-level data striping with dedicated parity | For large, sequential data requests | Doesnt support multiple simultaneous read and write requests |
| 4 | 3 | Block-level data striping with dedicated parity | Supports multiple read requests, if a disk fails the dedicated parity disk is used to create a replacement disk | Write requests are bottlenecked due to the dedicated parity drive
| 5 | 3 | Combination of data striping and parity | Supports multiple simultaneous reads and writes. Data is written across all | Write performance is slower than RAID O and 1 |

##### How does it work?

RAID takes data that is normally stored on a single disk and spreads it out among several drives. Except for RAID 0, if any single disk is lost, the user can recover data from the other disks where the data also resides.

RAID can also increase the speed of data recovery as multiple drives will be faster retrieving requested data than one disk doing the same.

##### RAID Data Storage 

A RAID solution can be either hardware-based or software-based. A hardware-based solution requires a specialized hardware controller on the system that contains the RAID drives, while software RAID is managed by utility software in the OS.

The following terms describe the various ways RAID can store data in the array of disks.

- Mirroring — Stores data, then duplicates and stores the same on a second drive.
- Striping — Writes data across multiple drives so that consecutive segments are stored on different drives.
- Parity — More precisely, striping with parity. After striping, checksums are generated to check that no errors exist in the striped data. These checksums are stored on a third drive.

Further RAID architectures exist, which mainly combine the above elements.

##### 2.6.8 Spanning Tree

Redundancy increases the availability of the infrastructure by protecting the network from a single point of failure, such as a failed network cable or a failed switch.

But when designers build physical redundancy into a network, loops and duplicate frames occur. Loops and duplicate frames have severe consequences for a switched network.

The Spanning Tree Protocol (STP) addresses these issues. Its basic function is to prevent loops on a network when switches interconnect via multiple paths. STP ensures that redundant physical links are loop-free and only one logical path runs between all destinations on the network. To do this, STP intentionally blocks redundant paths that could cause a loop.

Blocking the redundant paths is critical to preventing loops on the network. The physical paths still exist to provide redundancy, but STP disables these paths to prevent the loops from occurring. If a network cable or switch fails, STP recalculates the paths and unblocks the necessary ports to allow the redundant path to become active.

This animation shows the STP stages when a failure occurs.

1. PC1 sends a broadcast out onto the network.
2. The trunk link between S2 and S1 fails, resulting in disruption of the original path.
3. S2 unblocks the previously blocked port for Trunk2 and allows the broadcast traffic to traverse the alternate path around the network, permitting communication to continue.
4. If the link between S2 and S1 comes back up, STP again blocks the link between S2 and S3.

##### 2.6.9 Router Redundancy

The default gateway is typically the router that provides devices access to the rest of the network and/or to the internet. If there is only one router serving as the default gateway, it is a single point of failure. To avoid this, an organization can choose to install an additional standby router.

A redundancy protocol determines which router should take the active role in forwarding traffic; the forwarding router or the standby router? Each is configured with a physical IP address and a virtual router IP address. End devices use the virtual IP address as the default gateway

The forwarding router and the standby router use their physical IP addresses to send periodic messages. The purpose of these messages is to make sure both are still online and available.

If the standby router stops receiving these periodic messages from the forwarding router, it realizes it is the only router available and assumes the forwarding role for itself. Meanwhile, because the PCs on the network still communicate with the virtual router at 192.0.2.100, they stay online despite everything that has happened, since the virtual router now forwards to what was previously the standby router.

The ability of a network to dynamically recover from the failure of a device acting as a default gateway is known as **first-hop redundancy**, as we’ve seen in this scenario.

#### 2.6.10 Location Redundancy

An organization may also want to consider location redundancy, depending on its needs.

##### Synchronous Replication

- Synchronizes both locations in real time
- Requires high bandwidth
- Locations must be close together to reduce latency

##### Asynchronous Replication

- Not synchronized in real time but close to it
- Requires less bandwidth
- Sites can be further apart because latency is less of an issue

##### Point-in-Time Replication

- Updates the backup data location periodically, at certain points in time
- More bandwidth conservative because it does not require a constant connection

The correct balance between cost and availability will determine the correct choice for an organization.

#### 2.6.11 Resilient Design

Resiliency is the name given to the methods and configurations used to make a system or network tolerant of failure

- An example of resiliency is a network having redundant links between switches running STP. Although STP does provide an alternate path through the network if a link fails, the switchover may not be immediate if the configuration is not optimal, so these redundant links together with STP provide more resiliency.

- Routing protocols also provide resiliency, but fine-tuning can improve the switchover so that network users do not notice. Administrators should investigate non-default settings in a test network to see if they can improve network recovery times, thus leading to minimal disruption.

As seen in the above examples, resilient design is about more than just adding redundancy. It is critical to understand the business needs of the organization and then incorporate redundancy to create a resilient network.

#### 2.6.12 System and Data Backups

An organization can lose data if cybercriminals steal it, if equipment fails, or if a disaster or other error occurs, so it’s important to back up data regularly.

A data backup stores a copy of the information from a computer to backup media. When such media is removable, the operator then stores this backup media in a safe place.

Backing up data is one of the most effective ways of protecting against data loss. If the hardware fails, the user can restore the data from the backup once the system is functional again, or even when moving to a new system.

A sound security policy should include regular data backups. Backups are usually stored off-site to protect the data if anything happens to the main facility.

##### Frequency

Backups can take a long time. Sometimes, it is easier to make a full backup monthly or weekly and then do frequent partial backups of any data that has changed since the last full backup. However, having many partial backups increases the amount of time needed to restore data

##### Storage

For extra security, transport backups to an approved off-site storage location on a daily, weekly or monthly rotation, as required by the security policy

##### Security

Protect backups with passwords. The operator will enter the password before restoring the data from the backup media

##### Validation

Always validate backups to ensure the integrity of the data

#### 2.6.13 Designing High Availability Systems

High availability incorporates three major principles to achieve the goal of uninterupted access to data and services

##### Elimination or Reduction of Single Points of Failure

It is important to understand the ways to address a single point of failure. A single point of failure can be a central router or switch, a network service and even a highly skilled IT staff member.

What makes these single points of failure is the fact that a loss or failure of this system, process or person would have a very disruptive impact on the entire system, which should be avoided. Key, then, is to have processes, resources and components that minimize single points of failure.

High availability clusters are one way to provide redundancy. These clusters consist of a group of computers with identical configurations and access to the same shared storage. All servers take part in processing a service simultaneously. From the outside, the server group looks like one device, but the added benefit is that if a server within the cluster fails, the other servers continue to process the same service as the failed device.

##### Fault Tolerance

Fault tolerance enables a system to continue to operate if one or more of its components fail. Data mirroring is one example of fault tolerance. Should a fault occur, causing disruption in a device such as a disk controller, the mirrored system provides the requested data with no interruption in service apparent to the user.

##### System Resiliency 

System resiliency refers to the capability to maintain availability of data and operational processing despite attacks or disrupting events. Generally, this requires redundant systems, in terms of both power and processing, so that should one system fail, the other can take over operations without any break in service. System resiliency is more than hardened devices; it requires that both data and services be available, even when under attack.

#### 2.6.14 Power

A critical issue in protecting information systems is electrical power systems and power considerations. A continuous supply of electrical power is essential for today’s massive server and data storage facilities.

Here are some general rules in building effective electrical supply systems:

- Data centers should be on a different power supply from the rest of the building.
- Use redundant power sources — two or more feeds coming from two or more electrical substations.
- Implement power conditioning.
- Backup power systems are often required.
- Uninterruptible power supply (UPS) should be available to gracefully shut down systems.

##### Power Excess

- Spike - momentary high voltage
- Surge - prolonged high voltage

##### Power Loss 

- Fault - momentary loss of power
- Blackout - complete loss of power

##### Power Degradation

- Sag/dip - momentary low voltage
- Brownout - prolonged low voltage
- Inrush current - Initial surge of power

#### 2.6.15 Heating, Ventilation, and Air Conditioning (HAVC)

HVAC systems are critical to the safety of people and information systems in an organization's facilities. When designing modern IT facilities, these systems play a very important role in the overall stability and security.

##### HVAC System

HVAC systems control the ambient environment, including the temperature, humidity and airflow. This must be managed along with data components such as hardware, cabling, data storage, fire protection, physical security systems and power, and their needs

##### A product specifications document

Almost all physical computer hardware comes with environmental requirements that include acceptable temperature and humidity ranges. Environmental requirements are detailed in product specification documentation and/or physical planning guides. It is critical to observe these environmental requirements to prevent system failure and extend the life of IT systems

##### HVAC system contractor

Commercial HVAC systems and other building management systems now connect to the internet for remote monitoring and control. But recent events have shown such 'smart' systems also raise big security issues, as they are accessed and managed by HVAC system contractors or third-party vendors

##### Risks to the organization's security

Because the HVAC technicians need to be able to find information quickly, crucial data tends to be stored in many different places, making it accessible to even more people. This allows a wide network of individuals, including even associates of contractors, to gain access to the HVAC system. But the more people have access, the less secure these systems are, while their interruption can pose considerable risk to the organization's security

#### 2.6.17 Managing Threats to Physical Facilities

Organizations can implement various measures to manage threats to the physical facilities. For example:

- Access Control and Closed-Circuit TV (CCTV - Video Surveillance) coverage at all entrances
- Policies and procedures for guests visiting the facility
- Building security testing, including using both digital and physical means to covertly gain access
- Badge encryption for entry access
- Disaster recovery planning
- Business continuity planning
- Regular security awareness training
- Asset tagging system

### 2.7 Embedded and Specialized Systems

#### 2.7.2 Threats to Key Industry Sectors

Over the last decade, cyber attacks like Stuxnet proved that malware attacks could successfully destroy or interrupt critical infrastructures. The Stuxnet worm targeted Supervisory Control And Data Acquisition (SCADA) systems used to control and monitor industrial processes. SCADA and other Industrial Control Systems (ICSs) are used in manufacturing, production, energy and communications systems.

Actions that can be taken to prevent such attacks from occurring.

##### Stuxnet

A cyber attack like this could bring down or interrupt vital facilities like telecommunications, transportation systems or electrical power plants. It could also interrupt the financial services sector

Environments that use SCADA are vulnerable. When the SCADA architecture was first being developed, designers did not connect it to the traditional IT environment and the Internet. Therefore, they did not properly consider cybersecurity during the development phase of these systems

Now, however, organizations using SCADA systems recognize the value of data collection to improve operations and decrease costs. The resulting trend is to connect SCADA systems to the wider online IT infrastructure of the organization. This increases the vulnerability of industries using SCADA systems. 

To prevent attacks on these systems, you should segregate internal and external networks to separate the SCADA network from the organization's LAN.

#### 2.7.3 The Emergence of the Internet of Things

The Internet of Things (IoT) is the collection of technologies that enable various devices to connect to the Internet. The technological evolution associated with IoT is changing commercial and consumer environments.

IoT technologies enable people to connect billions of devices, such as cars, industrial machines, robots, appliances, locks, motors and entertainment devices, to name just a few. This technology affects the amount of data that needs to be protected. As users need to access these devices remotely, they are placed online, which increases the number of potential entry points to that local network in general.

Moreover, with the emergence of IoT, there is much more data to be managed and secured. All these devices, plus the expanded storage capacity and storage services offered through the cloud and virtualization, have led to the exponential growth of data. This data expansion created a new area of interest in technology and business called ‘Big Data.’

IoT devices greatly expand the cyber attack surface. In the IoT, thousands of new devices require access to networks in order to submit data and be managed and operated. Internet-connected smart devices have been infected with malware and used to launch some of the largest DDoS attacks in history. Therefore, IoT device security is extremely important. First, all IoT devices should be evaluated to ensure that they are able to update their firmware with security patches, preferably over wireless networks. In addition, default administrator credentials on these devices should always be changed from the default settings because these settings are publicly known.

#### 2.7.4 Embedded Systems

Embedded systems capture, store and access data. They pose unique security challenges due to their widespread adoption by both the corporate and the consumer world. They are used in smart TVs, HVAC control systems, medical devices and even automobiles.

##### Why are embedded systems vulnerable to attack?

Attacks against embedded systems exploit security vulnerabilities in the software and hardware components. They are susceptible to timing attacks, whereby attackers discover vulnerabilities by studying how long it takes the system to respond to different inputs. A timing attack is considered a side-channel attack.

This type of attack is based on information gained from the implementation of a system, rather than on weaknesses in the software. Timing information, power consumption, electromagnetic leaks or even sound can be that source of information.

##### How can embedded systems be protected?

One technique is to use **System on Chip (SoC)** technology. SoC technology is a Small Form Factor (SFF) hardware module — customer-grade examples include devices such as Raspberry Pi and Arduino. These devices are single-board computers that can be implemented using a Field-Programmable Gate Array (FGPA), an integrated circuit that can be programmed or modified in the field. This means that the user can make changes after deploying the device.

These devices have good processing power delivered in a small footprint. This reduces power consumption, lowers cost and offers better performance than traditional, larger components. SoC integrates a microcontroller, an application or microprocessor, and peripherals such as a GPU, a Wi-Fi module or a coprocessor. The processor can run an operating system such as Windows, Linux or Android.

Many of these SoC devices have poor authentication and/or they cannot be upgraded or patched. Due to the nature of these devices, a level of implied trust is necessary since there is no formal program in place to verify security controls.

#### 2.7.5 The Internet of Things (IoT)

The deployment and use of intelligent devices and sensors is one of the fastest growing sectors of information technology. The computer industry brands this sector as the Internet of Things (IoT).

Businesses and consumers use IoT devices to automate processes, monitor environmental conditions and alert the user of adverse conditions. Most IoT devices connect to a network via wireless technology. These include cameras, door locks, proximity sensors, lights, and other sensors used to collect information about an environment or the status of a device. Some manufacturers use IoT sensors to inform users that parts need to be replaced, components are failing or supplies are running out.

Organizations use IoT devices to track inventory, vehicles and personnel. IoT devices contain geospatial sensors. A user can globally locate, monitor and control environmental variables such as temperature, humidity, and lighting. IoT applications use a Real-Time Operating System (RTOS), a small operating system that allows for the rapid switching of tasks that focus on timing rather than throughput. Thes applications run with precise timing and high reliability. RTOS technology is found in wearables, medical devices, in-vehicle systems and home automation devices. 

The IoT industry poses a tremendous challenge to information security professionals because many IoT devices capture and transmit sensitive information. Vulnerabilities associated with RTOS include code injection, DoS attacks, and priority inversion (where a higher priority task is pre-empted by a lower priority task)

#### 2.7.6 Avatar

Using an IoT scanner such as Shodan is an easy way to tell whether a home automation device is vulnerable to attack. IoT devices communicate using short-range, medium-range or long-range methods and include cellular (4G, 5G), radio and Zigbee. Zigbee is a wireless set of protocols for Wireless Personal Area Networks (WPANs).

To secure IoT devices:

- Secure the wireless network.
- Know exactly which devices are communicating on your network.
- Know what each of the IoT devices on your network does.
- Install security software on devices where possible.
- Secure smartphones and mobile apps used to communicate with IoT devices.

#### 2.7.8 VoIP Equipment

VoIP uses the internet to make and receive phone calls

##### What equipment do you need?

You need an internet connection and a phone for VoIP. Several options are available for the phone set:

- A traditional phone with an adapter (the adapter acts as a hardware interface between a traditional, analog phone and a digital VoIP line)
- A VoIP-enabled phone
- VoIP software installed on a computer

##### Is VoIP secure?

Most consumer VoIP services use the internet for phone calls. Many organizations, though, use their private networks because they provide stronger security and service quality. VoIP security is only as reliable as the underlying network security. Cybercriminals target these systems to gain access to free phone services, to eavesdrop on phone calls, or to affect performance and availability.

##### How can you protect your VoIP service?

Implement the following countermeasures to secure VoIP:

- Encrypt voice message packets to protect against eavesdropping.
- Use SSH to protect gateways and switches.
- Change all default passwords.
- Use an intrusion detection system to detect attacks such as ARP poisoning.
- Use strong authentication to mitigate registration spoofing (cybercriminals routing all incoming calls for the victim to themselves), proxy impersonating (tricking the victim into communicating via a rogue proxy set up by the cybercriminals), and call hijacking (intercepting and rerouting calls to a different path before reaching their destination).
- Implement firewalls that recognize VoIP to monitor streams and filter abnormal signals.

When using VoIP equipment, remember that when the network goes down, voice communications will also go down.

#### 2.7.10 Special-Purpose Embedded Systems

Embedded systems work in a variety of industries. You can find special-purpose embedded devices in sectors such as the medical, automotive and aviation sectors.

##### Medical devices

Devices such as pacemakers, insulin pumps, medical implants and defibrillators are capable of wireless connectivity, remote monitoring and Near-Field Communication (NFC). Vulnerabilities in these medical devices can lead to patient safety issues, medical record leaks or the risk of granting access to the network to cybercriminals, who will move through it in search of a target.

##### Automotive

In-vehicle systems produce and store the data necessary for the operation of the vehicle along with its maintenance, safety protection and emergency contact transmission. Typically, a wireless interface connects to the Internet and to a diagnostic interface on board. Many vehicles record speed, location and braking maneuvers, and can then send the collected data to the driver’s insurance company.

Therefore, risks to in-vehicle communications include unauthorized tracking, wireless jamming and spoofing. To secure in-vehicle systems, implement the following countermeasures:

- Secure system software design practices
- Basic encryption for all communication between controllers
- Firewall implementation

##### Aviation

An aircraft has many embedded control systems such as its flight control system and communication system. Security issues include the use of hard-coded logon credentials, insecure protocols and backdoors.

In the same category, Unmanned Aerial Vehicles (UAVs), more commonly called drones, have been used in military, agricultural and cartography applications, among others. Drones are very useful for aerial photography, surveillance and surveying. However, drones are susceptible to hijacking, Wi-Fi attacks, GPS spoofing attacks, jamming and deauthentication attacks, which can allow an attacker to intercept or disable a drone and access its data.

#### 2.7.11 Deception Technologies

Organizations use deception technologies to distract attackers from production networks. They also use them to learn an attacker’s methods and to warn of potential attacks that could be launched against the network. Deception adds a fake layer to the organization’s infrastructure.

##### Honeypots

A **honeypot** is a decoy system that is configured to mimic a server in the organization's network. It is purposefully left exposed, to lure attackers. When an attacker goes after the honeypot, their activities are logged and monitored for later review. The honeypot distracts the attacker from the organization's real network resources.

An organization might even create a **honeynet**, a collection of honeypots, to mimic its network and distract attackers. Meanwhile, **honeyfiles** are dummy files that attract an attacker but do not contain any real information. 

##### DNS Sinkholes

A **DNS Sinkhole** prevents the resolution of hostnames for specified URLs and can push users away from malicious resources

## Module 3: Access Control

### 3.1 Access Controls

#### 3.1.2 Physical Access Controls

Physical access controls are actual barriers deployed to prevent direct physical contact with systems. The goal is to prevent unauthorized users from gaining physical access to facilities, equipment and other organizational assets.

For example, physical access control determines who can enter (or exit), where they can enter (or exit) and when they can enter (or exit).

Here are some examples of physical access controls:

- Guards to monitor the facility
- Fences to protect the perimeter
- Motion detectors to detect moving objects
- Laptop locks to safeguard portable equipment
- Locked doors to prevent unauthorized access
- Swipe cards to allow access to restricted areas
- Guard dogs to protect the facility
- Video cameras to monitor a facility by collecting and recording images
- Mantrap-style entry systems to stagger the flow of people into the secured area and trap any unwanted visitors
- Alarms to detect intrusion

#### 3.1.3 Logical Access Controls

Logical access controls are the hardware and software solutions used to manage access to resources and systems. These technology-based solutions include tools and protocols that computer systems use for identification, authentication, authorization and accountability.

Logical access control examples include:

- Encryption is the process of taking plaintext and creating ciphertext.
- Smart cards have an embedded microchip.
- Passwords are protected strings of characters.
- Biometrics are users’ physical characteristics.
- Access control lists (ACLs) define the type of traffic allowed on a network.
- Protocols are sets of rules that govern the exchange of data between devices.
- Firewalls prevent unwanted network traffic.
- Routers connect at least two networks.
- Intrusion detection systems monitor a network for suspicious activities.
- Clipping levels are certain allowed thresholds for errors before triggering a red flag.

#### 3.1.4 Administrative Access Controls

Administrative access controls are the policies and procedures defined by organizations to implement and enforce all aspects of controlling unauthorized access.

Administrative controls focus on personnel and business practices.

- **Policies** are statements of intent
- **Procedures** are the detailed steps required to perform an activity
- **Hiring practices** define the steps an organization takes to find qualified employees
- **Background checks** are a type of employee screening that includes information of past employment verification, credit history, and criminal history
- **Data classification** categorizes data based on its sensitivity
- **Security training** educates employees about the security policies at an organization
- **Reviews** evaluate an employee's job performance

#### 3.1.5 Administrative Access Controls in Detail

Let’s look into administrative access controls in more detail.

The concept of administrative access controls involves three security services: authentication, authorization and accounting (AAA).

These services provide the primary framework to control access, preventing unauthorized access to a computer, network, database or other data resource.

##### Authentication

The first A in AAA represents authentication. Authentication verifies the identity of each user, to prevent unauthorized access. Users prove their identity with a username or ID. In addition, users need to verify their identity by providing one of the following:

- Something they know (such as a password)
- Something they have (such as a token or card)
- Something they are (such as a fingerprint)
  
In the case of two factor authentication, which is increasingly becoming the norm, the system requires a combination of two of the above rather than just one to verify someone’s identity.

##### Authorization

Authorization services determine which resources users can access, along with the operations that users can perform.

Some systems accomplish this by using an access control list, or an ACL. An ACL determines whether a user has certain access privileges once the user authenticates. Just because you can log onto the corporate network does not mean that you have permission to use the high-speed color printer, for example.

Authorization can also control when a user has access to a specific resource. For example, employees may have access to a sales database during work hours, but the system locks them out afterhours.

##### Accounting

Not related to financial accounting, accounting in AAA keeps track of what users do — including what they access, the amount of time they access resources, and any changes they make.

For example, a bank keeps track of each customer account. An audit of that system can reveal the time and amount of all transactions and the employee or system that executed the transactions. Cybersecurity accounting services work the same way. The system tracks each data transaction and provides auditing results. System administrators can set up computer policies to enable system auditing.

The concept of AAA is like using a credit card. The credit card identifies who can use it, how much that user can spend and accounts for items or services the user purchased.

Cybersecurity accounting tracks and monitors in real time.

#### 3.1.6 What is Identification 

Identification enforces the rules established by the authorization policy. Every time access to a resource is requested, the access controls determine whether to grant or deny access.

A unique identifier ensures the proper association between allowed activities and subjects. A username is the most common method used to identify a user. A username can be an alphanumeric combination, a personal identification number (PIN), a smart card or biometric — such as a fingerprint, retina scan or voice recognition.

A unique identifier ensures that a system can identify each user individually, therefore allowing an authorized user to perform the appropriate actions on a particular resource.

Cybersecurity policies and the sensitivity of the information or systems determine which identification controls should be used and how stringent they should be.

#### 3.1.8 Federated Identity Management

Federated identity management refers to multiple enterprises that let their users use the same identification credentials to gain access to the networks of all enterprises in the group. Unfortunately, this broadens the scope and increases the probability of a cascading effect should an attack occur.

Generally speaking, a federated identity links a subject’s electronic identity across separate identity management systems, such as being able to access several websites using the same social login credentials.

The goal of federated identity management is to share identity information automatically across castle boundaries. From the individual user’s perspective, this means a single sign-on to the web.

It is imperative that organizations scrutinize the identifying information shared with partners, even within the same corporate group, for example. The sharing of social security numbers, names and addresses may allow identity thieves the opportunity to steal this information from a partner to perpetrate fraud. The most common way to protect federated identity is to tie login ability to an authorized device.

#### 3.1.9 Authentication Methods

As we mentioned earlier, users prove their identity with a username or ID. In addition, users need to verify their identity by providing one of the following.

##### What you know

Passwords, passphrases or PINs are all examples of something that the user knows. Passwords are the most popular method used for authentication.

The terms passphrase, passcode, passkey and PIN are all generically referred to as password. A password is a string of characters used to prove a user’s identity. If this string of characters relates back to a user (for instance, if it is their name, birthdate or address), it will be easier for cybercriminals to guess this user’s password.

Several publications recommend that a password be at least eight characters. Users should not create a password that is so long that it is difficult to memorize, or conversely, so short that it becomes vulnerable to password cracking. Passwords should contain a combination of upper and lowercase letters, numbers, and special characters.

Users need to use different passwords for different systems because if a criminal cracks the user’s password once, the criminal will have access to all of the user’s accounts. A password manager can help you create and use strong passwords — and means that you do not have to remember each of these passwords, either. 

##### What you have

Smart cards and security key fobs are both examples of something that users have in their possession that can be used for authentication purposes.

A smart card is a small plastic card, about the size of a credit card, with a small chip embedded in it. The chip is an intelligent data carrier, capable of processing, storing and safeguarding data. Smart cards contain private information, such as bank account numbers, personal identification, medical records and digital signatures, using encryption to keep data safe while providing a means to authenticate.

A security key fob is a device that is small enough to attach to a keyring. In most cases, security key fobs are used for two factor authentication (2FA), which is much more secure than a username and password combination.

For example, let’s say you want to access your e-banking, which uses two factor authentication. First, you enter your username (identification). Then, the password, which is your first authentication factor. Then, you need a second one, because it's 2FA. You enter a PIN or card to your security fob, and it displays a number. Proving that you have access to this device, which was issued to you, this number is the second factor, which you then enter to log in to the e-banking account, in this example.

##### Who you are

Unique physical characteristics, such as a fingerprint, retina or voice, which identify a specific person are called biometrics. Biometric security compares physical characteristics against stored profiles to authenticate users. In this case, a profile is a data file containing known characteristics of an individual. The system grants the user access if their characteristics match saved settings. A fingerprint reader is a common biometric device.

There are two types of biometric identifiers:

- Physiological characteristics — fingerprints, DNA, face, hands, the retina or ear features.
- Behavioral characteristics — patterns of behavior such as gestures, voice, gait or typing rhythm.

Biometrics is becoming increasingly popular in public security systems, consumer electronics and point-of-sale applications. Implementing biometrics involves a reader or scanning device, software that converts the scanned information into digital form and a database that has biometric data stored for comparison.

#### 3.1.10 Multi-Factory Authentication

As we’ve touched upon earlier, multi-factor authentication uses at least two methods of verification — such as a password and something you have, for example, a security key fob. This can be taken a step further by adding something you are, such as a fingerprint scan.

Multi-factor authentication can reduce the incidence of online identity theft because it means knowing a password will not give cybercriminals access to a user’s account.

For example, an online banking website might require a password and a one-off PIN that the user receives on his or her smartphone. In this case, your first factor is your password, and your second factor the temporary PIN, because it proves you have access to what is registered as your phone.

Withdrawing cash from an ATM is another, simple example of multi-factor authentication as the user must have the bank card as well as know the PIN before the ATM will dispense cash.

Note that two factor authentication (2FA) is a method of multi-factor authentication that entails two factors in particular, but the two terms are often used interchangeably.

#### 3.1.12 Authorization 

Authorization controls what a user can and cannot do on the network after successful authentication. After a user proves their identity, the system checks to see what network resources the user can access and what they can do with the resources.

##### When to implement authorization

Authorization uses a set of attributes that describes the user’s access to the network, to answer the question, ‘What read, copy, edit, create and delete privileges does this user have?’

The system compares these attributes to the information contained within the authentication database, determines a set of restrictions for that user, and delivers it to the local device where the user is connected.

Authorization is automatic and does not require users to perform additional steps after authentication. System administrators have set the network up to implement authorization immediately after the user authenticates.

##### Using authorization

Defining authorization rules is the first step in controlling access. An authorization policy establishes these rules.

A group membership policy defines authorization based on users’ membership in a specific group. All employees of an organization may have a swipe card, for example, which provides access to the premises, but it might not allow access to a server room. It may be that only senior-level employees and IT team members may access the server room with their swipe cards.

An authority-level policy defines access permissions based on an employee’s position within the organization.

#### 3.1.15 Implementing Accountability

##### What is accountability?

Accountability traces an action back to a person or process making this change to a system. Accountability then collects this information and reports the usage data. The organization can use this data for such purposes as auditing or billing. The collected data might include the log-in time for a user, whether the user login was a success or failure, or what network resources the user accessed. This allows an organization to trace actions, errors and mistakes during an audit or investigation.

##### Implementing accountability

Implementing accountability consists of technologies, policies, procedures and education. Log files provide detailed information based on the parameters chosen. For example, an organization may look at the log for login failures and successes. Login failures can indicate that a criminal tried to hack an account, and login successes tell an organization which users are using what resources and when.

The organization’s policies and procedures spell out what actions should be recorded and how the log files are generated, reviewed and stored.

##### Providing accountability

Data retention, media disposal and compliance requirements all provide accountability. Many laws require the implementation of measures to secure different data types. These laws guide an organization on the right way to handle, store and dispose of data. The education and awareness of an organization’s policies, procedures and related laws can also contribute to accountability.

### 3.2 Access Control Concepts

#### 3.2.1 Zero Trust Security

Zero trust is a comprehensive approach to securing all access across networks, applications, and environments. This approach helps secure access from users, end-user devices, APIs, IoT, microservices, containers, and more. It protects an organization’s workforce, workloads, and the workplace. The principle of a zero trust approach is, “never trust, always verify.” Assume zero trust any time someone or something requests access to assets. A zero trust security framework helps to prevent unauthorized access, contain breaches, and reduce the risk of an attacker's lateral movement through a network.

Traditionally, the network perimeter, or edge, was the boundary between inside and outside, or trusted and untrusted. In a Zero trust approach, any place at which an access control decision is required should be considered a perimeter. This means that although a user or other entity may have successfully passed access control previously, they are not trusted to access another area or resource until they are authenticated. In some cases, users may be required to authenticate multiple times and in different ways, to gain access to different layers of the network.

The three pillars of zero trust are workforce, workloads, and workplace.

##### Zero Trust for the Workforce

This pillar consists of people (e.g., employees, contractors, partners, and vendors) who access work applications by using their personal or corporate-managed devices. This pillar ensures only the right users and secure devices can access applications, regardless of location.

##### Zero Trust for Workloads

This pillar is concerned with applications that are running in the cloud, in data centers, and other virtualized environments that interact with one another. It focuses on secure access when an API, a microservice, or a container is accessing a database within an application.

##### Zero Trust for the Workplace

This pillar focuses on secure access for any and all devices, including on the internet of things (IoT), that connect to enterprise networks, such as user endpoints, physical and virtual servers, printers, cameras, HVAC systems, kiosks, infusion pumps, industrial control systems, and more.

#### 3.2.2 Access Control Models

An organization must implement proper access controls to protect its network resources, information system resources, and information.

A security analyst should understand the different basic access control models to have a better understanding of how attackers can break the access controls.

The various types of access control methods.

##### Discretionary Access Control (DAC)

- This is the least restrictive model and allows users to control access to their data as owners of that data.
- DAC may use ACLs or other methods to specify which users or groups of users have access to the information.

##### Mandatory Access Control (MAC)

- This applies the strictest access control and is typically used in military or mission critical applications.
- It assigns security level labels to information and enables users with access based on their security level clearance.

##### Role-based Access Control (RBAC)

- Access decisions are based on an individual’s roles and responsibilities within the organization.
- Different roles are assigned security privileges, and individuals are assigned to the RBAC profile for the role.
- Roles may include different positions, job classifications or groups of job classifications.
- Also known as a type of **non-discretionary access control**.

##### Attribute-based Access Control (ABAC)

ABAC allows access based on attributes of the object (resource) to be accessed, the subject (user) accessing the resource, and environmental factors regarding how the object is to be accessed, such as time of day.

##### Rule-based Access Control (RBAC)

- Network security staff specify sets of rules regarding or conditions that are associated with access to data or systems.
- These rules may specify permitted or denied IP addresses, or certain protocols and other conditions.
- Also known as **Rule Based RBAC.**

##### Time-based Access Control (TAC)

TAC Allows access to network resources based on time and day.

Another access control model is the principle of least privilege, which specifies a limited, as-needed approach to granting user and process access rights to specific information and tools. The principle of least privilege states that users should be granted the minimum amount of access required to perform their work function.

A common exploit is known as privilege escalation. In this exploit, vulnerabilities in servers or access control systems are exploited to grant an unauthorized user, or software process, higher levels of privilege than they should have. After the privilege is granted, the threat actor can access sensitive information or take control of a system.

#### 3.2.3 Network Access Control (NAC) Systems

Network access control (NAC) systems support access management by enforcing organizational policies regarding the people and devices that are attempting to access the network. NAC systems allow cybersecurity professionals to monitor the users and devices that are attached to the network, and manually control access as required.

Network access control systems provide the following capabilities:

- Rapidly enforcing access policies that have been created for different operational conditions.
- Recognizing and profiling connected users and devices to prevent malicious software on non-compliant systems from causing damage.
- Providing secure access to network guests, often through registration portals.
- Evaluating device compliance with security policies by user type, device type, and operating system prior to permitting network access.
- Mitigating security incidents by blocking, isolating, or repairing non-compliant devices.

Because BYOD and IoT networking greatly expand the network attack surface, NAC system automation features make focused control of network access by such devices practical. The NAC system is configured to enforce organizational policies. The relevant policies are enacted to permit or deny network access according to a wide range of factors that the NAC system detects on the devices that are attempting access. Without NAC systems it would be impossible for cybersecurity personnel to evaluate the thousands of devices that could attempt to access the network.

NAC is an important component of a zero-trust security architecture that enforces security policy compliance with all devices and users that attempt to access the network.

### 3.3 Account Management

#### 3.3.2 Account Types

An organization should not share accounts for privileged users, administrators or applications. The administrator account should only be used to administer a system. If a user accesses a malware-infected website or opens a malicious email while using the administrator account, this would put the organization at risk.

Administrators must be aware of the default group and user accounts that might be installed by an operating system. Knowing about these accounts will help an administrator decide which should be permitted and which of these accounts should be disabled.

This is because default accounts such as the guest or administrator account can be a security risk in older systems as attackers are familiar with the default settings used. To improve security, always replace any default accounts and make sure that all account types require a password.

It's important to properly manage accounts to maintain security

- On hiring a new employee, create the identity profile, register the employee's computer and mobile devices, and enable access to the organization's network. As the Identity Provider (IdP), the organization is responsible for authenticating their identity
- Disable or deactivate any accounts that are no longer needed and retrieve and organizational data or applications from the user's devices
- Grant a user no more access than is necessary to perform assigned tasks (least privilege)
- Review user access to identify any access control adjustments that need to be made
- Use time-of-day restrictions to control when a user can log in
- Use location restrictions to control where a device or user can log in from
  - Geofencing is used to trigger an action when a user enters or exits a geographic boundary
  - Geolocation identifies a device based on its geographic location
  - Geotagging adds an identifier to something based on the location (like a photo taken on a smartphone tagged with the coordinates of where the photo was taken)

#### 3.3.3 Privileged Accounts

Cybercriminals target privileged accounts. Why? Because these are the most powerful accounts in the organization with elevated, unrestricted access to systems. Administrators use these accounts to deploy and manage operating systems, applications and network devices.

Organizations should adopt robust practices for securing privileged accounts.

- Identify and reduce the number of privileged accounts.
- Enforce the principle of least privilege. The principle means that users, systems, and processes only have access to resources (networks, systems and files) that are absolutely necessary to perform their assigned function.
- Revoke access rights when employees leave or change jobs.
- Eliminate shared accounts with passwords that do not expire.
- Secure password storage.
- Eliminate shared credentials for multiple administrators.
- Automatically change privileged account passwords every 30 or 60 days.
- Record privileged sessions.
- Implement a process to change embedded passwords for scripts and service accounts.
- Log all user activity.
- Generate alerts for unusual behavior.
- Disable inactive privileged accounts.
- Use multi-factor authentication for all administrative access.
- Implement a gateway between the end user and sensitive assets to limit network exposure to malware.

Continuously securing and locking down privileged accounts is critical to the security of the organization. Regularly evaluate this process and make adjustments to improve protection.

#### 3.3.4 File Access Control

Let’s take a closer look at how permissions can help secure data.

Permissions are rules configured to limit folder or file access for an individual or a group. Users should be limited to only the resources they need on a computer system or network. For example, they should not be able to access all files on a server if they only need access to a single folder. It may be easier to provide access to the entire drive, but it is more secure to limit access to only the folder they need. This is the principle of least privilege and closely connected to the concept of ‘need to know’ access. Limiting access to resources also prevents cybercriminals from accessing those resources if the user’s computer becomes infected.

##### Full Control

Users can:

- See the contents of a file or folder.
- Change and delete existing files and folders.
- Create new files and folders.
- Run programs in a folder.

##### Modify

Users can change and delete existing files and folders but cannot create new ones.

##### Read and Execute

Users can see the contents of existing files and folders and can run programs in a folder.

##### Write

Users can create new files and folders and make changes to existing files and folders.

##### Read

Users can see the contents of a folder and open files and folders.

If an administrator denies an individual or group permissions to a network share, this will override any other permission settings.

For example, if the administrator denies someone permission to a network share, the user cannot access that share, even if the user is the administrator or part of the administrator group. The local security policy must outline the resources and the type of access allowed for each user and group.

After parent folder permissions have been set, folders and files created inside the parent folder inherit its permissions. The location of data and the action performed on it also determine the permission propagation:

- Data moved to the same volume will keep the original permissions. 
- Data copied to the same volume will inherit new permissions. 
- Data moved to a different volume will inherit new permissions.
- Data copied to a different volume will inherit new permission.

#### 3.3.7 Account Policies in Windows

In most networks that use Windows computers, an administrator configures Active Directory with domains on a Windows server. Windows computers that join the domain become domain members.

The administrator configures a domain security policy that applies to all domain members. For example, account policies are automatically set when a user logs in to Windows.

When a computer is not part of an Active Directory domain, the user configures policies through Windows Local Security Policy. In all versions of Windows except Home edition, enter ‘secpol.msc’ at the Run command to open the Local Security Policy tool.

##### Password Policy

An administrator can configure user account policies such as password policies and lockout policies.

In the example shown, users must change their passwords every 90 days and use each new password for at least one day. Passwords must contain eight characters and three of the following four categories: uppercase letters, lowercase letters, numbers and symbols. Lastly, the user can reuse a password after 24 unique passwords. 

This is just an example; different password policies can be set, depending on organizational requirements and needs.

##### Account Lockout Policy

An account lockout policy locks an account for a set duration when too many incorrect login attempts occur.

For example, the policy shown here allows the user to enter the wrong username and/or password five times. After five attempts, the account locks users out for 30 minutes. After 30 minutes, the number of attempts resets to zero and the user can attempt to log in again.

##### Audit Policies

More security settings are available by selecting the ‘local policies’ folder in Windows. An audit policy creates a security log file used to track the following events:

- Account logon events.
- Audit account management.
- Directory service access.
- Object access.
- Policy changes.
- Privilege use.
- Process tracking.
- System events.

#### 3.3.8 Authentication Management

Authentication and authorization issues include unencrypted credentials, incorrect permissions and access violations. But how do you keep cybercriminals out while still making it easy for authorized users to log in? Authentication management aims to ensure secure sign in while still providing ease of use.

- A **Single Sign On (SSO)** solution allows the user to use one set of login credentials to authenticate across multiple applications. This way, the user only needs to remember one strong password. 
- **OAuth** is a standard that enables a user’s account information to be used by third-party services such as Facebook or Google.  
- A **password vault** can protect and store the user’s credentials with a single strong password required to access them.
- Many organizations implement **Knowledge-Based Authentication (KBA)** to provide a password reset should a user forget their password. KBA is based on personal information known by the user or a series of questions.

#### 3.3.10 Hash-Based Message Authentication Code (HMAC)

Hash-Based Message Authentication Code (HMAC) uses an encryption key with a hash function to authenticate a web user. Many web services use basic authentication, which does not encrypt the username and password during transmission. Using HMAC, the user sends a private key identifier and an HMAC. The server looks up the user’s private key and creates an HMAC. The user’s HMAC must match the one calculated by the server.

VPNs using IPsec rely on HMAC functions to authenticate the origin of every packet and provide data integrity checking.

Cisco products use hashing for entity authentication, data integrity, and data authenticity purposes

- Cisco IOS router use hashing with secret keys in an HMAC-like manner to add authentication information to routing protocol updates
- IPsec gateways and clients use hashin algorithms, such as MD5 and SHA-1 in HMAC mode, to provide packet integrity and authenticity
- Cisco software images on Cisco.com have an MD5-based checksum available so that customers can check the integrity of downloaded images





















