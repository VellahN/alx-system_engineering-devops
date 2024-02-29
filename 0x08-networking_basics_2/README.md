The hosts file is a plain text file that all operating systems use to translate hostnames (also known as web addresses or URLs) into IP addresses

In computer networking, localhost is a hostname that refers to the current computer used to access it. The name localhost is reserved for loopback purposes.[1] It is used to access the network services that are running on the host via the loopback network interface. Using the loopback interface bypasses any local network interface hardware.

The local loopback mechanism may be used to run a network service on a host without requiring a physical network interface, or without making the service accessible from the networks the computer may be connected to. For example, a locally installed website may be accessed from a Web browser by the URL http://localhost to display its home page.

IANA, who allocate IP addresses globally, have allocated the single IP address 0.0.0.0[1] to RFC 1122 section 3.2.1.3. It is named as "This host on this network".

RFC 1122 refers to 0.0.0.0 using the notation {0,0}. It prohibits this as a destination address in IPv4 and only allows it as a source address under specific circumstances.

A host may use 0.0.0.0 as its own source address in IP when it has not yet been assigned an address, such as when sending the initial DHCPDISCOVER packet when using DHCP.
