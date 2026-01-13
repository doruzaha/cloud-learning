## Day 10 Security Groups vs Networks ACLs 

## Security Groups (concept + proof)

Security Groups are stateful firewalls at instance level.
If Inbound traffic is allowed, return traffic is automatically allowed.
No explicit deny rules.

Security Groups = stateful( return traffic allowed automatically)
NACLs = stateless ( must allow inbound and outbound)

- Instance level firewall
- Stateful
- Allow rules only
- Blocks traffic before OS

# Test 
- Removed SSH ( port 22)
- SSH failed immediately
- SSh restored

# Network ACLs:
- Subnet-level firewall
- Stateless
- Allow and deny rules
- Rule order matters
