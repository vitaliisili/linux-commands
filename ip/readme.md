# ip

*The `ip` command is a powerful tool for configuring network interfaces that any Linux system administrator should know. <br/> 
It is used to bring interfaces up or down, assign and remove addresses and routes, manage ARP cache, and much more.*

## Syntax
```bash
ip [ OPTIONS ] OBJECT { COMMAND | help }
```

## Options

- `l` : Network device.
- `a` : Protocol (IP or IPv6) address on a device.
- `addrl` : Label configuration for protocol address selection.
- `n` : ARP or NDISC cache entry.
- `r` : Routing table entry.
- `ru` : Rule in routing policy database.
- `m` : Multicast address.
- `mr` : Multicast routing cache entry.
- `t` : Tunnel over IP.
- `x` : Framework for IPsec protocol.

## Examples

### 1. Displays info about all network interfaces
```bash
ip a
```

### 2. Delete a ARP entry
```bash
ip neigh del 192.168.1.5 dev eth1
```

### 3. Show routing table
```bash
ip r list
```

### 4. Add a new route
```bash
ip route add 192.168.1.0/24 via 192.168.1.254
```