# Exam Tips

## Writeups and Guides

### From TJNull

[https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html](https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html)

### From /u/tristanlogd

![[Pasted image 20210418203944.png]]

Source: [https://www.reddit.com/r/oscp/comments/k7x4o1/just_passed_oscpmy_journey_and_tips/](https://www.reddit.com/r/oscp/comments/k7x4o1/just_passed_oscpmy_journey_and_tips/)

### From JohnJHacking

[[https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/](https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/)]([https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/](https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/))

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

## Taking Breaks

Take regular breaks!

Try to set yourself regular timers to avoid rabbit holes, and move on after 30 minutes of trying something without progress.