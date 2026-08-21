# Network Defense Notes

## Module 1: Understanding Defense

### 1.1 Defense-in-Depth
#### 1.1.1 Assets, Vulnerabilities, Threats

As a cybersecurity analyst, it is my job to secure the assets of the organization's network. To do this, I must:

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


































