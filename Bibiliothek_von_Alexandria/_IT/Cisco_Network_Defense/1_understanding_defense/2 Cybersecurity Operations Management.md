# Configuration Management
Configuration management refers to identifying, controlling and auditing the implementation and any changes made to a system’s established baseline.

The baseline configuration includes all the settings that you configure for a system which provide the foundation for all similar systems — like a template of sorts.

For instance, those responsible for deploying Windows workstations to users must install the required applications and set up the system settings according to a documented configuration. This is the baseline configuration for Windows workstations within this organization.

Documented configuration resources might include the following:
- Network maps 
- cabling 
- wiring diagrams
- application configuration specifications

Hardening the operating system is an important part of making sure that systems have secure configurations. Configuring log files along with auditing, changing default account names and passwords, and implementing account policies and file-level access control are all used to create a secure OS.

# Log files
A log records all events as they occur. Log entries make up a log file, with each log entry containing all the information related to a specific event. Accurate and complete logs are very important in cybersecurity.

For example, an audit log tracks user authentication attempts, while an access log records details on requests for specific files on a system. Monitoring system logs will therefore help us determine how an attack occurred and which of the defenses deployed were successful — and which were not.

As an increasing number of log files are generated for computer security purposes, organizations should consider a log management process. Management of computer security log data should determine the procedures for the following:

- Generating log files
- Transmitting log files
- Storing log files
- Analyzing log data
- Disposing of log data

# Operating System Logs and Application Security Logs
**OS Logs:**
Operating system logs record events that are linked to actions that have to do with the operating system. System events include the following:

- Client requests and server responses such as successful user authentications

- Usage information that contains the number and size of transactions in a given period of time

**Application Security Logs:**
Organizations use network-based and/or system-based security software to detect malicious activity.

This software generates a security log to provide computer security data. These logs are useful for performing auditing analysis and identifying trends and long-term problems. Logs also enable an organization to provide documentation showing that it complies with laws and regulatory requirements.

# Protocol Analyzer
Packet analyzers, otherwise known as packet sniffers, intercept and log network traffic.

The packet analyzer captures each packet, looks at the values of various fields in the packet and analyzes its content. It can capture network traffic on both wired and wireless networks.

Packet analyzers perform the following functions:

- Traffic logging
- Network problem analysis
- Detection of network misuse
- Detection of network intrusion attempts
- Isolation of exploited systems

Protocol Analyzer are (but not limited to):
- Wireshark
- TCPdump
- Ettercap
- Kismet
- Ngrep
- Ntop
- EtherApe
