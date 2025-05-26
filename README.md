
# Nmap Scan Results

This repository contains the results of a TCP SYN scan performed using Nmap on a local network.

## Scan Details

- *Command used*:  
  nmap -sS -T4 192.168.163.0/24 -oN scan_results.txt

- *Date*: May 26, 2025
- *Scan Type*: Stealth (SYN) Scan

## Example Findings
Nmap scan report for 192.168.163.1
Host is up (0.0011s latency).
Not shown: 999 filtered tcp ports (no-response)
PORT    |  STATE| SERVICE
6881/tcp| open  | bittorrent-tracker
MAC Address: 00:50:56:C0:00:08 (VMware)


## Security Notes

- Port 22 (SSH): Should have strong password or key-based auth.
- Port 445 (SMB): Common malware target; disable if unnecessary.
- Port 8080: Often used for web admin panels; restrict access.

## Tools Used

- Nmap
- Optional: Wireshark for packet analysis
