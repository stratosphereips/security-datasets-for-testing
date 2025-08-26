# 002-zeek-scenario-port-scanning

- Source: Stratosphere Laboratory
- Notes: one client 172.16.1.11 performing multiple scans using Nmap in different local networks (172.16.1.0/24, 192.168.1.0/24, 10.0.2.0/24).
- Tool: Nmap
- Format: JSON


- Target: 1.1.1.1

## Command


`nmap -sS -n -v -d 1.1.1.1`

```
root@Matterhorn:~# nmap -sS -n -v -d 1.1.1.1
Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-08-26 09:37 UTC
PORTS: Using ports open on 0% or more average hosts (TCP:1000, UDP:0, SCTP:0)
--------------- Timing report ---------------
  hostgroups: min 1, max 100000
  rtt-timeouts: init 1000, min 100, max 10000
  max-scan-delay: TCP 1000, UDP 1000, SCTP 1000
  parallelism: min 0, max 0
  max-retries: 10, host-timeout: 0
  min-rate: 0, max-rate: 0
---------------------------------------------
Initiating Ping Scan at 09:37
Scanning 1.1.1.1 [4 ports]
Packet capture filter (device eno1): dst host 147.32.80.37 and (icmp or icmp6 or ((tcp) and (src host 1.1.1.1)))
We got a ping packet back from 1.1.1.1: id = 51154 seq = 0 checksum = 14381
Completed Ping Scan at 09:37, 0.01s elapsed (1 total hosts)
Overall sending rates: 359.10 packets / s, 13645.75 bytes / s.
Initiating SYN Stealth Scan at 09:37
Scanning 1.1.1.1 [1000 ports]
Packet capture filter (device eno1): dst host 147.32.80.37 and (icmp or icmp6 or ((tcp) and (src host 1.1.1.1)))
Discovered open port 80/tcp on 1.1.1.1
Discovered open port 8080/tcp on 1.1.1.1
Discovered open port 443/tcp on 1.1.1.1
Discovered open port 53/tcp on 1.1.1.1
Discovered open port 8443/tcp on 1.1.1.1
Discovered open port 2000/tcp on 1.1.1.1
Discovered open port 5060/tcp on 1.1.1.1
Completed SYN Stealth Scan at 09:37, 4.86s elapsed (1000 total ports)
Overall sending rates: 410.51 packets / s, 18062.62 bytes / s.
Nmap scan report for 1.1.1.1
Host is up, received echo-reply ttl 55 (0.00069s latency).
Scanned at 2025-08-26 09:37:15 UTC for 5s
Not shown: 992 filtered tcp ports (no-response)
PORT     STATE  SERVICE    REASON
53/tcp   open   domain     syn-ack ttl 56
80/tcp   open   http       syn-ack ttl 55
113/tcp  closed ident      reset ttl 63
443/tcp  open   https      syn-ack ttl 55
2000/tcp open   cisco-sccp syn-ack ttl 63
5060/tcp open   sip        syn-ack ttl 63
8080/tcp open   http-proxy syn-ack ttl 56
8443/tcp open   https-alt  syn-ack ttl 55
Final times for host: srtt: 687 rttvar: 818  to: 100000

Read from /usr/bin/../share/nmap: nmap-protocols nmap-services.
Nmap done: 1 IP address (1 host up) scanned in 4.97 seconds
           Raw packets sent: 1997 (87.844KB) | Rcvd: 10 (416B)
```
