## Nmap Scan Analysis

**Target:** testphp.vulnweb.com

**Command used:**
nmap -sS -sV -Pn -T4 testphp.vulnweb.com

**Observations:**
- Host is reachable
- All 1000 TCP ports are filtered (no-response)
- Reverse DNS indicates AWS (ec2 instance)

**Interpretation:**
- Likely firewall/security group is dropping probes
- Direct service enumeration is restricted
- Network-level attack surface is minimized

**Risk / Impact:**
- Reduced exposure to direct port-based attacks
- Limited visibility may hide misconfigurations behind the filter

**Recommendation:**
- Allow only required ports explicitly
- Audit firewall/security group rules
- Enable logging/monitoring for dropped traffic