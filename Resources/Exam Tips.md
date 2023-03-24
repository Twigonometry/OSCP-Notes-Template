## Writeups and Guides

### From TJNull

[https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html](https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html)

### From /u/tristanlogd

![[Pasted image 20210418203944.png]]

Source: [https://www.reddit.com/r/oscp/comments/k7x4o1/just_passed_oscpmy_journey_and_tips/](https://www.reddit.com/r/oscp/comments/k7x4o1/just_passed_oscpmy_journey_and_tips/)

### From JohnJHacking

[[https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/](https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/)]([https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/](https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/))

### My Writeup

I did my OSCP back in 2021, before the [new course](https://www.offsec.com/offsec/oscp-exam-structure/) was rolled out, which shifted focus away from Buffer Overflows . It has since then been [updated again](https://www.offsec.com/offsec/pen-200-2023/), with a wealth of new content and expansions on old modules. Unfortunately, even if you paid for the OSCP in the past you can't access the new content, despite already forking out over a grand...

I think this change towards AD-focused content was a positive one, and will modernise the OSCP content a lot. However, I can no longer guarantee that this notes template is laid out in the optimal way for the new content, labs, and exam. You might need to do some tweaking!

Neverthless, you can read my writeup of my OSCP experience here: https://www.mac-goodwin.com/blog/cyber/2021/10/16/oscp-experience.html

The TLDR is that I learned a lot from my OSCP and thoroughly enjoyed the experience, but I believe the criticism of OffSec's predatory pricing is pretty much warranted. However, the course was still very valuable to me and made me a better hacker - if you can afford it, I recommend it, but remember there are lots of cheaper courses out there (including the [PEH course](https://academy.tcm-sec.com/p/practical-ethical-hacking-the-complete-course)). Overall, the OSCP is still one of the most recognised certifications out there, and I can attest to its 'HR power' in job interviews and recruiting. OffSec critics don't like to admit it, but the letters next to your name grab the attention of employers, even if they don't mean you're a top-notch hacker.

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