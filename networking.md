---
title: Notes on networking (Extra)
---

# Networking Refresher
- IP Networks are split in 5 classes. 
    - A Range: 0.0.0.0 to 127.255.255.255
        - 128 Class A networks can be assigned (Each Entity assigned gets 16.8 Million IPs)
        - from 0.X.X.X to 127.X.X.X
        - Alloted entities control 3 bits of Address
        - /8 in CIDR
    - B Range: 128.0.0 to 191.255.255.255
        - 16,000 networks can be assigned (Each entity gets 65,536 IPS)
        - 128.0.X.X, 128.1.X.X to 191.255.X.X 
        - Alloted Entities control 2 bits of Address
        - /16 in CIDR
    - C Range: 192.0.0.0 to 223.255.255.255
        - 256 Addresses per network
        - Alloted Entities cotrol only last bit of address.
        - /32 in CIDR
    - D & E Ranges are ignored for SAA

- Certain Ranges are allocated for private use. 
    - 1 Class A (10.0.0.0 to 10.255.255.255)
    - 16 Class B (172.16.0.0 to *172.31*.255.255)
    - 256 Class C (192.168.0.0 to 192.168.255.255)

## CIDR (Classles inter-domain routing)
- Network Address + / + prefix (size of network.)
- Prefix of one nuber is half than prefix of the number before it.
- E.g. Prefix of 16 have double the networks than 17 and half the networks than 15s.
- Spliting a network of IPs to smaller networks using prefixes is called subnetting.
    - E.g. Splitting the range of ips of /16 to 4 networks of /18 is called subnetting.  
