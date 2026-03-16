# DNS & ICMP Network Traffic Investigation

## Scenario
Users reported they could not access the website www.yummyrecipesforme.com and received the error message "destination port unreachable."

Network traffic was analyzed using tcpdump to determine the cause of the issue.

## Tools Used
- tcpdump

## Network Protocols Observed
- DNS
- UDP
- ICMP

## Investigation Findings

1. The client system sent DNS queries to a DNS server using UDP port 53.
2. Instead of receiving a DNS response, the DNS server returned ICMP error messages.
3. The ICMP message stated: "udp port 53 unreachable."
4. This indicates that the DNS service on the server was not available or not listening on port 53.

## Impact

Because the DNS query failed, the browser could not resolve the domain name to an IP address. As a result, the website could not load.

## Root Cause

DNS service on the server was unavailable or misconfigured, causing UDP port 53 to be unreachable.

## Recommendation

- Verify that the DNS service is running.
- Confirm that UDP port 53 is open and listening.
- Check firewall rules that may be blocking DNS traffic.
- Monitor DNS traffic for abnormal activity.

## Key Skills Demonstrated

- Network traffic analysis
- Packet inspection
- DNS troubleshooting
- Identifying ICMP error responses
