
**tl;dr use the links in this README**
#### [Linux Terminal](Linux%20Terminal/)
- [Linux Commands Cheat Sheet](https://docs.google.com/document/d/1vJxoHrjW607NJDLC1Zln1llrEIqrS6Ea3j9ihJTdblg/) ⇒ all the actually useful Linux commands, including the ones mentioned in the NCAE Cyber Sandbox Tutorials
  - For anyone who wants it, the Windows counterpart is here: [Windows Commands Cheat Sheet](https://docs.google.com/document/d/1CGgADAOZQuMXAyzXVeXRNhQ_PPBYliMXCy-4RNE0UMw/)
- [Printing Tricks](https://github.com/RedefiningReality/Cheatsheets/blob/main/Parsing%20Command%20Output.md) ⇒ commands related to working with command line output: grep, sed, cut, tr, etc. This is also linked in the Linux Commands Cheat Sheet for convenience
- [Keyboard Shortcuts](Linux%20Terminal/Keyboard%20Shortcuts.md) ⇒ window management, navigating history, and rerunning previous commands with select modifications, all through keyboard shortcuts
#### [Linux Defence](Defence/)
- [Attack Vectors](Defence/Attack%20Vectors.md) ⇒ attack vectors by service and the most basic privilege escalation attacks
- [Defence Checklist](Defence/Defence%20Checklist.md) ⇒ Illinois Tech's approach to cyber defence competitions
- [Auditing Commands](Defence/Auditing%20Commands.md) ⇒ various methods to log all commands executed
- [Closing Ports (the right way)](Defence/Port%20Closing%20Flowchart.png) ⇒ I'm tired of people thinking a firewall is the solution to all their problems... actually remove services you don't need!
- [Linux Services and Defence Cheat Sheet](https://docs.google.com/document/d/1DikLS0jAhuflCj3bOlbh5ZIJE6Ou4WkyIxMN0t2ZqU0/) ⇒ all the service setup commands mentioned in the NCAE Cyber Sandbox Tutorials but in the form of a reference sheet + some defence ideas
#### [NCAE Checklists](NCAE%20Checklists/)
- [Linux Checklist](NCAE%20Checklists/Linux%20Checklist.pdf) ⇒ the "boilerplate" Linux defence checklist Illinois Tech used for competitions - we took this one and use it to create separate checklists for each machine
  - **To Do:** fix one-liner for removing extra users (in rare cases, it deletes service users also) and add [command line auditing](Defence/Auditing%20Commands.md) with auditd
- [DNS Configuration](NCAE%20Checklists/DNS%20Configuration.pdf) ⇒ bind9 is a mess, so here are all the changes you need to make written out
- [Recovery Plan](NCAE%20Checklists/Recovery%20Plan.pdf) ⇒ booting into recovery to reset root password and making backups of sensitive files (eg. website source code)
#### [Practice Materials](Practice%20Materials/)
- [iptables Template](Practice%20Materials/iptables-template.sh) ⇒ iptables is even yuckier than bind9, so here's a template you can follow when setting up iptables rules
  - iptables is the "lowest-level" firewalling solution, and that gives it some distinct advantages over ufw or firewalld - namely, red team can just remove those when they inevitably compromise you
- [Illinois Tech Practice Range Network Diagram](Practice%20Materials/practice.jpg) ⇒ 
  - The actual infrastructure we use for hosting our practice range is fully documented [here](https://github.com/RedefiningReality/Proxmox-Remote-Management/blob/main/Web.md), and if you're a visual learner you can watch [this series](https://youtube.com/playlist?list=PLSpsCUl2cY8at6Dr0c28G6-yC1exBnqrR) on YouTube instead.

If you want to play around with some Python scripts I wrote for logging all command line history and monitoring logins, feel free to check out my [Linux Defence Scripts](https://github.com/RedefiningReality/Linux-Defence-Scripts) repo. They're pretty basic, and if I were to rewrite them now I'd probably take a different approach, but they work!
