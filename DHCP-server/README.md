DHCP Configuration Lab

Summary

This lab demonstrates how to configure DHCP on a Cisco router to automatically assign IPv4 addresses to hosts within a network.


The router is configured as a DHCP server to provide clients with:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server

The lab also includes excluded addresses to reserve specific IPs for network devices.

Configuration

- Configure the router as a DHCP server.
- Exclude reserved IP addresses.
- Create a DHCP pool.
- Configure the network address.
- Configure the default gateway.
- Configure the DNS server.
- Verify that end devices receive their IP configuration automatically.

Verification

DHCP operation was verified by checking the IP configuration on the end devices and testing connectivity using "ping".

Key Commands

ip dhcp excluded-address <start-ip> <end-ip>

ip dhcp pool <POOL-NAME>
 network <network-address> <subnet-mask>
 default-router <gateway-ip>
 dns-server <dns-ip>

Result

All DHCP clients successfully received valid IPv4 addresses and network configuration automatically from the Cisco router.