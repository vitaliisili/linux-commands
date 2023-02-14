# ping

*The `ping` command is used to test the connectivity between two networked devices. It sends <br/> 
Internet Control Message Protocol (ICMP) echo requests to a network host and reports the responses received.*

## Syntax
```bash
ping [OPTION]... DESTINATION
```

## Options

- `-c` `COUNT`: Send COUNT number of echo requests.
- `-f`: Flood ping. Outputs packets as fast as they come back or one hundred times per second. Only the super-user may use this option.
- `-I` `INTERFACE`: Specify the network interface to use.
- `-i` `WAIT`: Wait WAIT seconds between sending each packet. The default is to wait for one second between each packet.
- `-L`: Suppress loopback of multicast packets.
- `-n`: Numeric output only. No attempt will be made to look up symbolic names for host addresses.
- `-w` `TIMEOUT`: Specify a timeout, in seconds, before ping exits regardless of how many packets have been sent or received.
- `-W` `TIMEOUT`: Specify a timeout, in seconds, for the round-trip time to the target host.

## Examples

### 1. To ping the network host with IP address `192.168.1.1`
```bash
ping 192.168.1.1
```

### 2. To ping the network host with hostname `www.google.com`
```bash
ping www.google.com
```

### 3. To ping the network host with IP address `192.168.1.1` for 10 times
```bash
ping -c 10 192.168.1.1
```