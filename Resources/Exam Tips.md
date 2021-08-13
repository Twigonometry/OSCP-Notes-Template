# Exam Tips

## Taking Screenshots

Proof screenshots for the exam [need to include](https://help.offensive-security.com/hc/en-us/articles/360040165632-OSCP-Exam-Guide#screenshot-requirements) the following:
- IP address of the machine (to prove you aren't in a container)
- Contents of `proof.txt`

From within the directory that holds `proof.txt` (usually `C:\Users\Administrator\Desktop` on Windows and `/root` on Linux), the following command lets you view the required info in one line:
- Windows: `type proof.txt && ipconfig`
- Linux: `cat proof.txt && ip addr`

Alternative commands are:
- `ifconfig`
- `netstat -ie` (not accepted in the exam, but can be used for your own personal purposes in the lab machines if above commands do not work)