# Intro to Dynamic Host Configuration Protocol (DHCP) Overview Guide

**TODO**: A brief introductory guide to Dynamic Host Configuration Protocol (DHCP).

#### Table of Contents

1. [DHCP Explained](#explained)
2. [DHCP Pros and Cons](#pros)
3. [The Four Step Handshake](#handshake)
4. [Relay Agents](#relay)
5. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="explained">DHCP Explained</a>

(TODO)

<hr />

## 2. <a name="pros">DHCP Pros and Cons</a>

(TODO)

<hr />

## 3. <a name="handshake">The Four Step Handshake</a>

The DHCP 4-way handshake process involves the checking off, in sequence, of four flags: *DHCPDISCOVER*, *DHCPOFFER*, *DHCPREQUEST*, and *DHCPACK*. These flags (logically serving as a boolean true/false variable) represent the process in which a client device requests an IP address, a DHCP server offers one in response to the client, the client accepts the IP address offer and requests that it indeed wants it, and the DHCP server recognizes the lease of the IP address.

1) **DHCPDISCOVER:** The client sends out a DHCPDISCOVER broadcast so that it can request an IP address (or renew one that it is already leasing).
2) **DHCPOFFER:** The DHCP server responds to this effort with a DHCPOFFER message that includes the configuration parameters of an available IP address, a gateway address, and a subnet mask, as well as relevant DNS server information.
3) **DHCPREQUEST:** The client sends this (and, specifically, broadcasts this message out to servers) to confirm to the server that it wants to accept the DHCP offer.
4) **DHCPACK:** 'ACK' is short for 'ACKNOWLEDGMENT': the server confirms the lease and handles the assignment of the IP address.

<hr />

## 4. <a name="relay">Relay Agents</a>

(TODO)

<hr />

## 5. <a name="supplemental">Supplemental Resources</a>

* *[Official Red Hat Guide to Configuring a DHCP Server](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/7/html/networking_guide/sec-dhcp-configuring-server)*
* *[Official Cisco Guide to Configuring a DHCP Server in Cisco IOS](https://www.cisco.com/en/US/docs/ios/12_4t/ip_addr/configuration/guide/htdhcpsv.html#wp1084769)*
* *[Official Microsoft Guide to Configuring a DHCP Server in Windows Server](https://learn.microsoft.com/en-us/windows-server/networking/technologies/dhcp/quickstart-install-configure-dhcp-server?tabs=powershell)*
