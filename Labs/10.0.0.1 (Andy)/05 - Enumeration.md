# Andy Enumeration

## nmap

I ran the following command:

```bash
$ nmap -sC -sV -oA nmap/andy 10.0.0.1
```

Key Findings:
- Web Server on port 80
- SMB on port 445

### All Ports

I also ran a full port scan:

```bash
$ nmap -p- nmap/andy-allports 10.0.0.1
```

It found no new ports.

## SMB Enumeration

### SMBMap

I ran `smbmap` to enumerate shares.

### SMBClient

I connected with `smbclient` to read files.

## Gobuster

I ran the following gobuster scan:

```bash
$ gobuster dir -u http://10.0.0.1 -w /usr/share/seclists/Discovery/Web-Content/raft-small-words.txt -x php
```

It found the following interesting pages:
- `/remote.php`