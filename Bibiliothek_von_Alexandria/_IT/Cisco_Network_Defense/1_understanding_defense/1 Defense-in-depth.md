# Identifying Assets
The collection of all the devices and information owned or managed by the organization are assets. The assets constitute the attack surface that threat actors could target. These assets must be inventoried and assessed for the level of protection needed to thwart potential attacks.

Asset management consists of inventorying all assets, and then developing and implementing policies and procedures to protect them. This task can be daunting considering many organizations must protect internal users and resources, mobile workers, and cloud-based and virtual services.

# Asset Classification
The most critical information needs to receive the highest level of protection and may even require special handling.
A labeling system can be used to determine how valuable, how sensitive, and how critical the information is.

**Step 1:** Determinate Asset category: 
- Information assets
- Software assets
- Physical asset
- Services

**Step 2:** Establish asset accountability by identifying the owner of each information asset and each piece of software:
- Identify the owner for all information assets.
- Identify the owner for all application software.

**Step 3:** Determinate the criteria for classification:
- Confidentiality
- Value
- Time
- Access rights
- Destruction

**Step 4:** Implement a classification schema:
- Adopt a consistent way of identifying information to ensure uniform protection and easier monitoring.

# Asset Standardization
Asset standards identify specific hardware and software products used by an organization.

When a failure occurs, prompt action helps to maintain both access and security. If an organization does not standardize its hardware selection, personnel may need to scramble to find a replacement component. Non-standard environments require more expertise to manage, and they increase the cost of maintenance contracts and inventory.

# Asset Lifecycle Stages
For cybersecurity specialists, part of the job is to manage information assets and related systems throughout that asset’s lifecycle.

**Procurement:**
The organization purchases the assets based on the needs identified from data gathered to justify the purchase.

The asset is added to the organization’s inventory.

**Deployment:**
The asset is assembled and inspected to check for defects or other problems. Staff perform tests and install tags or barcodes for tracking purposes.

The asset moves from inventory to in-use.

**Utilization:**
This is the longest stage of the cycle. The asset’s performance is continuously checked. Upgrades, patch fixes, new license purchases and compliance audits are all part of the utilization stage.

**Maintenance:**
Maintenance helps to extend an asset’s productive life. Staff may modify or upgrade the asset.

**Disposal:**
At the end of the asset’s productive life, it must be disposed of. All data must be wiped from the asset. Disposal may include dismantling an asset for parts. Any parts that can cause an environmental hazard must be disposed of according to local guidelines.

# Identify Vulnerabilities
Threat identification provides an organization with a list of likely threats for a particular environment. When identifying threats, it is important to ask several questions:

- What are the possible vulnerabilities of a system?
- Who may want to exploit those vulnerabilities to access specific information assets?
- What are the consequences if system vulnerabilities are exploited and assets are lost?

For instance: 
The threat identification for an e-banking system would include:

- **Internal system compromise -** The attacker uses the exposed e-banking servers to break into an internal bank system.
- **Stolen customer data -** An attacker steals the personal and financial data of bank customers from the customer database.
- **Phony transactions from an external server -** An attacker alters the code of the e-banking application and makes transactions by impersonating a legitimate user.
- **Phony transactions using a stolen customer PIN or smart card -** An attacker steals the identity of a customer and completes malicious transactions from the compromised account.
- **Insider attack on the system -** A bank employee finds a flaw in the system from which to mount an attack.
- **Data input errors -** A user inputs incorrect data or makes incorrect transaction requests.
- **Data center destruction -** A cataclysmic event severely damages or destroys the data center.

Identifying vulnerabilities on a network requires an understanding of the important applications that are used, as well as the different vulnerabilities of that application and hardware. This can require a significant amount of research on the part of the network administrator.

# Identifying Threats
Organizations must use a defense-in-depth approach to identify threats and secure vulnerable assets. This approach uses multiple layers of security at the network edge, within the network, and on network endpoints.

A simple topology of a defense-in-depth approach would be:
- **Edge router -** The first line of defense is known as an edge router (R1 in the figure). The edge router has a set of rules specifying which traffic it allows or denies. It passes all connections that are intended for the internal LAN to the firewall.
- **Firewall -** The second line of defense is the firewall. The firewall is a checkpoint device that performs additional filtering and tracks the state of the connections. It denies the initiation of connections from the outside (untrusted) networks to the inside (trusted) network while enabling internal users to establish two-way connections to the untrusted networks. It can also perform user authentication (authentication proxy) to grant external remote users access to internal network resources.
- **Internal router -** Another line of defense is the internal router (R2 in the figure). It can apply final filtering rules on the traffic before it is forwarded to its destination.

Routers and firewalls are not the only devices that are used in a defense-in-depth approach. Other security devices include Intrusion Prevention Systems (IPS), Advanced Malware Protection (AMP), web and email content security systems, identity services, network access controls and more.

In the layered defense-in-depth security approach, the different layers work together to create a security architecture in which the failure of one safeguard does not affect the effectiveness of the other safeguards.

# The Security Onion and The Security Artichoke
There are two common analogies that are used to describe a defense-in-depth approach.

**Security Onion:**
A common analogy used to describe a defense-in-depth approach is called “the security onion.” As illustrated in figure, a threat actor would have to peel away at a network’s defenses layer by layer in a manner similar to peeling an onion. Only after penetrating each layer would the threat actor reach the target data or system.
**Note:** The security onion described on this page is a way of visualizing defense-in-depth. This is not to be confused with the Security Onion suite of network security tools.

![[../../../IMG/IMG_IT/Security_Onion.png]]

**Security Artichoke:**
The changing landscape of networking, such as the evolution of borderless networks, has changed this analogy to the “security artichoke”, which benefits the threat actor.

As illustrated in the figure, threat actors no longer have to peel away each layer. They only need to remove certain “artichoke leaves.” The bonus is that each “leaf” of the network may reveal sensitive data that is not well secured.

For example, it’s easier for a threat actor to compromise a mobile device than it is to compromise an internal computer or server that is protected by layers of defense. Each mobile device is a leaf. And leaf after leaf, it all leads the hacker to more data. The heart of the artichoke is where the most confidential data is found. Each leaf provides a layer of protection while simultaneously providing a path to attack.

Not every leaf needs to be removed in order to get at the heart of the artichoke. The hacker chips away at the security armor along the perimeter to get to the “heart” of the enterprise.

While internet-facing systems are usually very well protected and boundary protections are typically solid, persistent hackers, aided by a mix of skill and luck, do eventually find a gap in that hard-core exterior through which they can enter and go where they please.

![[../../../IMG/IMG_IT/Security_Artichoke.png]]

# Defense in Depth Strategies
To make sure data and infrastructure remain secure, an organization should create different layers of protection.

**Layering:**
To make sure data and information remains available, an organization must set up different layers of protection, creating a barrier of multiple defenses that work together to prevent attacks. A good example of layering is an organization storing its top-secret documents on a password-protected server in a locked building that is surrounded by an electric fence.

Defense in depth does not provide an impenetrable shield, but it will help an organization minimize risk by staying one step ahead of cybercriminals.

**Limiting:**
 An organization should restrict access so that each user only has the level of access required to do their job.

An organization should have the right tools and settings, such as file permissions, in place to limit access, as well as the right procedural measures, which define specific steps for doing anything that can affect security. For example, a limiting procedure which requires employees to always consult sensitive documents in a room which has CCTV, ensures that they would never remove such documents from the premises.

**Diversity:**
The layers must be different so that if one layer is penetrated, the same technique will not work on all the others which would compromise the whole system. Furthermore, an organization will normally use different encryption algorithms and authentication systems to protect data in different states.

To accomplish the goal of diversity in defenses, organizations can use security products by different companies as different factors of authentication, such as a swipe card from one company and a fingerprint reader manufactured by a different company — as well as varied security measures, such as time-delay locks on cabinets and supervision by a security staff member upon unlocking it.

**Obscurity:**
Obscuring information can also protect data and information. An organization should not reveal any information that cybercriminals can use to identify which Operating System (OS) a server is running, or the type or make of equipment or software it uses.

Error messages or system information should not contain any details that a cybercriminal could use to determine what vulnerabilities are present. Concealing certain types of information makes it more difficult for cybercriminals to attack.

**Simplicity:**
Complexity does not necessarily guarantee security. If an organization implements complex systems that are hard to understand and troubleshoot, this may backfire. If employees do not understand how to configure a solution properly, such as setting up their account using an unnecessarily complex process, this may make it just as easy for cybercriminals to compromise those systems.

A security solution should be simple from the inside, but complex on the outside.