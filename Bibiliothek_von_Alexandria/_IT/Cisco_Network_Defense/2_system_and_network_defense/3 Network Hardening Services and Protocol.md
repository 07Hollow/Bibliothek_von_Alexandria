Cybercriminals use vulnerable network services to attack a device or to use it as part of an attack. To check for insecure network services, use a port scanner to detect open ports on a device. A port scanner sends a message to each port and waits for a response, which indicates how the port is used and whether it is open.

But beware, cybercriminals also use port scanners for this same reason! Securing network services ensures that only necessary ports are exposed and available.

# DHCP
DHCP uses a server to assign an IP address and other configuration information to network devices. In effect, the device gets a permission slip from the DHCP server to use the network. Attackers can target DHCP servers to deny access to devices on the network, but security measures like DHCP snooping prevent rogue DHCP servers from providing IP addresses to clients by validating messages from sources that are not trusted.

A security checklist for DHCP:

- Physically secure the DHCP server.
- Apply any software patches.
- Locate the DHCP server behind a firewall.
- Monitor DHCP activity by reviewing DHCP logs.
- Maintain a strong antivirus solution.
- Uninstall any unused services and applications.
- Close unused ports.

# DNS
DNS translates a URL or website address, such as https://sebastiansimon.netlify.app, into a numerical IP address. When users type a web address into the address bar, the DNS server will recognize the IP address. Attackers can target DNS servers to deny access to network resources or redirect traffic to rogue websites. Use secure service and authentication between DNS servers to protect them from these attacks.

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

# ICMP
Network devices use ICMP to send error messages, that a requested service is not available or the host could not reach the router, for example.

The ping command is a network utility that uses ICMP to test the reachability of a host on a network. Ping sends ICMP messages to the host and waits for a reply. Cybercriminals can alter the use of ICMP to run reconnaissance, denial of service (DoS) and covert channel attacks. Many networks filter ICMP requests to prevent such attacks.

# RIP
RIP is a routing protocol that limits the number of hops from source to destination that are allowed in a network path. The maximum number of hops allowed for RIP is fifteen. RIP is used to exchange routing information about which networks each router can reach and how far away those networks are.

RIP calculates the best route based on hop count, but cybercriminals can also target routers and the RIP protocol. Such attacks on routing services can affect performance and availability, some attacks can even result in traffic redirection. Use secure services with authentication and implement system patching and updates to protect routing services.

# NTP
Having the correct time within networks is important. Correct timestamps accurately track network events such as security violations. Additionally, clock synchronization is critical for the correct interpretation of events within syslog data files as well as for digital certificates.

Network Time Protocol (NTP) is a protocol that synchronizes network computer system clocks. NTP allows network devices to synchronize their time settings with an NTP server. Cybercriminals attack timeservers to disrupt secure communication that depends on digital certificates and to hide attack information. Use NTP Authentication to verify that the server is trusted.