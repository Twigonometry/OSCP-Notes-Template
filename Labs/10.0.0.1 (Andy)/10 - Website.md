# Website

Screenshot of website index page:

![[Pasted image 20210813173305.png]]

## Enumerating Tech Stack

### Examining Source

### Enumerating PHP Version

## Gobuster

I ran [[Labs/10.0.0.1 (Andy)/05 - Enumeration#Gobuster|Gobuster]] - it found `/remote.php`.

## Remote File Inclusion

I found a Remote File Inclusion vulnerability on the `/remote.php` site.

### Testing RFI

Outline process of testing parameters on page for RFI...

### Gaining a Shell

Outline process of debugging shell execution...

Summary of commands used to gain shell:
- Start a listener with `sudo nc -lnvp -413`
- Visit the following url: ...