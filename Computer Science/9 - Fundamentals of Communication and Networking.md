
## Components of a Packet
- Packet sequence number (allows the packets to be re-ordered when they arrive at their destination)
- Source IP address
- Destination IP address
- Source MAC address
- Destination MAC address
- Data that is being sent
- Error checking methods (like a checksum)

## Packet Switching
1. Network Interface Card (NIC) receives a message to send data
2. NIC splits the data into equally sized packets and numbers them
3. Packets are routed to the local ISP, each one is checked for errors on arrival
4. Packets are routed to the next router. Depending on the bandwidth, congestion and other factors packets may take different routes.
5. Packets arrive at the ISP of the destination computer.
6. Packets arrive at the destination and the TCP protocol re-orders the packets into the correct sequence.
7. Protocol bits are stripped from the packets, the original data is passed onto the application that needs it.

## Routable vs Non-routable IPs

**Routable IP** $-$ IP addresses assigned to devices connected directly to the public/global internet and are unique

**Non-routable IP** $-$ IP addresses assigned to devices internally on private networks.

## NAT & Port forwarding

**Network Address Table (NAT)** $-$ responsible for converting IP addresses as they pass over the boundary between public and private address spaces

**Port forwarding** $-$ allows remote computers (outside the network) to connect to a specific computer or service within a private local network.

## Gateways
**Gateway** $-$ a device that allows for the transmission of data across dissimilar networks (e.g. networks that use different protocols)