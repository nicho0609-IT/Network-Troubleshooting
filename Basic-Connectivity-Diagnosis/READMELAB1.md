# Lab1: Basic Connectivity Diagnosis

## Ticket

User wants to Diagnose his network connectivity

## Objective

Diagnose network connectivity using basic networking tools.

## Tools Used in this diagnosis
```
- ipconfig
- ping
- nslookup
- tracert
- netstat
```
## investigation Process

# 1. Check IP configuration

### command used: 

```
ipconfig
```
### Screenshot:

## ipconfig output

![ipconfig-output](Screenshots/ipconfig%20output.png)

Verified that the system has a valid IPv4, subnet mask, and default gateway.

# 2. Test local TCP/IP stack

### command used: 
```
ping 127.0.0.1
```
### Screenshot:

### TCPIP Stack
![TCIP stack](screenshots/TCPIP%20Stack%20.png)

This confirms that the local TCP/IP is functioning correctly.

# 3. Test connectivity to the router

### command used: 
```
ping 192.168.1.1
```

## Router Ping
![Router Ping](screenshots/Router%20Ping.png)

This confirms that the system can reach the local network gateway.

# 4. Test connectivity to internet 

### command used: ##
```
ping 8.8.8.8
```

## Internet Ping
![Network Ping](screenshots/Network%20Ping.png)

This confirms that the system has external network connectivity.

# 5. Test DNS resolution 

### command used: 
```
nslookup google.com
```
## DNS Resolution

![DNS Resolution](screenshots/DNS%20Resolution.png)

DNS Resolution is working properly.

# 6. Packet Route

### Command used:
```
tracert google.com
```

## Tracert Route
![Tracertroute](screenshots/Traceroute.png)

Packet route and intermediate gateways are functioning correctly.

# 7. Port 443 Behavior

### command used:
```
netstat -ano
```

## Connection Port 443
![Port 443](screenshots/433%20Port.png)

Established connections over port 443 (HTTPS) indicate that secure web traffic is functioning normally.

# Conclusion
All connectivity tests were successful:

- IP configuration is valid
- Local TCP/IP stack is functioning
- Gateway connectivity is operational
- External network connectivity is confirmed
- DNS resolution is working
- Network route to external hosts is reachable
- HTTPS connections over port 443 are established

No network issues were identified during this diagnosis.

[def]: screenshots/ipconfi-output.png
[def2]: Screenshots/ipconfig%20output.png