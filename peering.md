# Peering

- This page describe the peering policy for network AS4242421045 (CIRNO-AS).
- Open peering policy on all nodes if no additional restriction applied.
- This page is still under construction, information may be changed quicky.

## Submitting a Request
- For now, only wireguard protocol is supported. More protocol may be supported in the future.
- Please provide these following information when sending your request:
  - Your ASN
  - Your clearnet address (or domain) and port number
  - Your DN42 IPv4 address
  - Your Dn42 IPv6 link-local address
  - If Multiprotocol BGP is required; default is Enabled
  - Your wireguard public key
  - The node ID you are trying to connect
  - Any additional information, special configuration, etc.
  
## Network Description
- as-name: `CIRNO-AS`
- description: Cirno's Perfect Network Class
- ASN: `4242421045`
- mnt: `STANG-MNT`
- Listening port: last five digits of your ASN
- Link-local IPv6 address: `fe80::1045`
- Contact: `$(echo ZG40MkBjaGlyZWlkZW4uZGV2 | base64 -d)`

## Nodes
#### APAC

| ID | 1001 |
| -- | --|
| Location | Hong Kong, HK |
| Connectivity | IPv4 + IPv6, 10Gbps |
| Clearnet IP address | `hosthatch-hkg35.node.koishi.eu.org` |
| DN42 IPv4 address | `172.21.81.65` |
| DN42 IPv6 address | `fd6e:2659:5811::1045:1001` |
| Wireguard public key | `aWKi/AUj605XoFZ/byMEQkI+5QwbxY+CbzM6/Sc/DXM=` |


| ID | 1002 |
| -- | --|
| Location | Tokyo, JP |
| Connectivity | IPv4 + IPv6, 1Gbps |
| Clearnet IP address | `virmach-nrt25.node.koishi.eu.org` |
| DN42 IPv4 address | `172.21.81.66` |
| DN42 IPv6 address | `fd6e:2659:5811::1045:1002` |
| Wireguard public key | `3etwl8AAbiKwI2k6KY6Q0iBC8qpJiT6n01NiuDldH00=` |

#### NA
Under construction
#### EU
Under construction

## Achievements
- [x] [Initialization](https://git.dn42.dev/dn42/registry/pulls/2428)
- [x] Setup your first node
- [x] More nodes, connect them [internally](https://jlu5.com/blog/dn42-multiple-servers-ibgp-igps)
- [ ] Make your network clever: deploy OSPF
- [ ] Really need to start a session between all two nodes? Deploy RR (BGP Route Reflector)
- [ ] DNS time! Register your own `.dn42` domain
- [ ] Is this a route? Setup web based looking glass on your nodes
- [ ] IX! Connect to an IX
- [ ] BGP community
- [ ] Automatic! Auto-peer system
- [ ] Monitor node status via Prometheus (Telegraf + InfluxDB) + Grafana

...


