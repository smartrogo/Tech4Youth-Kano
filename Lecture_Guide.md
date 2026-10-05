# Cybersecurity Training
## Beginner Lecture and Practical Guide

**Four weeks | 20 training days | 40 guided practicals**

This guide follows the uploaded curriculum and is designed for learners who are new to cybersecurity. Each week is a self-contained teaching unit. Teach the core lesson, discuss the everyday example and live scenario, then complete the daily practicals in order.

## How to teach each day

Use the course's five-hour model:

| Time | Activity |
|---|---|
| 45 minutes | Review, simple explanation and learning goal |
| 75 minutes | Teach the main idea with examples and questions |
| 45 minutes | Trainer demonstrates on a screen |
| 105 minutes | Learners complete the two practicals for the day |
| 30 minutes | Review results, ask questions and check understanding |

Give learners time to follow each step. Demonstrate first, let them repeat it, and invite them to explain what they observed. They do not need prior coding or cybersecurity experience.

### Safety rules for every practical

- Work only on your own device, a device you have clear permission to use, or an instructor-provided lab.
- Never test a school, business, public website, Wi-Fi network or another person's account without written permission and a defined scope.
- Do not open suspicious links or attachments. Use the screenshots or sample messages supplied by the instructor.
- Use made-up names and sample data. Do not put real passwords, private messages or personal information in class worksheets.
- Do not disable antivirus, firewall, updates or other protective controls. If a task requires an administrator, ask the trainer.
- Stop and tell the trainer if a screen or result differs from the instructions.

### Simple words to remember

| Word | Beginner meaning |
|---|---|
| Asset | Something valuable to protect, such as a laptop or student record |
| Threat | Something that could cause harm |
| Vulnerability | A weakness that could be used to cause harm |
| Risk | How likely harm is and how serious it would be |
| Control | A step that lowers risk |
| Evidence | Information that helps show what happened |
| Scope | The exact devices, accounts and activities approved for a test |

---

# Week 1 — Foundations
## Days 1–5: Understand systems and common threats

**Phase:** Foundations  
**Duration:** 5 training days / 25 contact hours  
**Audience:** Complete beginners  
**Approach:** Practical-first • Instructor demonstration • Guided practice

> **Week 1 theme:** Understand the system before you learn how to secure it.

## Week 1 learner outcomes

By the end of Week 1, learners should be able to:
1. Explain assets, threats, vulnerabilities, risks and controls using everyday examples.
2. Describe confidentiality, integrity and availability (CIA).
3. Find basic operating-system, account, file and network information on their own computer.
4. Use beginner Linux commands to navigate and search a practice file.
5. Recognize common phishing signs and write a clear, safe report.

### Week overview

By Friday, learners should be able to explain basic cyber risks, find common information about their own computer and network, use a few Linux commands, and report suspicious messages safely.

### Core lesson

Cybersecurity means protecting devices, accounts, networks and information. A useful way to discuss protection is the **CIA triad**:

- **Confidentiality:** only the right people can see the information.
- **Integrity:** information stays correct and is not changed without permission.
- **Availability:** people can use the information or service when they need it.

An asset may have a weakness. A threat may take advantage of that weakness. Risk is the possible harm; a control reduces the chance or impact. For example, a weak email password is a vulnerability, an account thief is a threat, account takeover is a risk, and multi-factor authentication (MFA) is one control.

Computers use an operating system such as Windows or Linux to manage programs, files, users and hardware. Networks let devices communicate. An IP address helps route network traffic; DNS helps find the IP address associated with a website name. Linux commands let a user ask the computer for information by typing.

Attackers also target people. Phishing messages try to make someone reveal information, open a file or send money. Pause, inspect, and verify through a separate trusted method.

### Everyday example

A learner's phone is lost on a bus. If the screen has no lock, private photos may be seen (confidentiality). If someone changes a saved assignment, it may no longer be trustworthy (integrity). If the learner cannot sign in to class, the information is unavailable (availability). A screen lock, backups and account recovery options each help in a different way.

### Live scenario — “The urgent school payment”

A staff member receives a message that appears to come from the head teacher: “I am in a meeting. Pay this supplier now and keep it confidential.” Ask the class to identify the asset, threat, warning signs, possible impact and safe control. The safe response is not to use the contact details in the message: pause and verify with the head teacher using a known phone number or in person, then report the message using the organization's normal channel.

### Five-day plan

| Day | Lesson | Practical numbers |
|---|---|---|
| 1 | Cybersecurity, risk, CIA and ethics | 1–2 |
| 2 | Computers, accounts, files and basic security | 3–4 |
| 3 | Networks and troubleshooting | 5–6 |
| 4 | Linux basics | 7–8 |
| 5 | Threat awareness and safe reporting | 9–10 |

## Day 1 — Cybersecurity foundations, risk and ethics

### Practical 1 — Make a personal asset-and-risk map

**You need:** paper or a notes app. **Use:** only made-up examples; do not write passwords.

1. List five things you use or care about, such as a phone, school email, photos, mobile money account or assignment.
2. For each one, write one thing that could go wrong, such as loss, a guessed password or a scam message.
3. Write what the harm could be: private information exposed, money lost, or work unavailable.
4. Add one protection, such as a screen lock, MFA, backup or asking an adult to verify a payment request.
5. Circle the protection that would help the most and explain why.

**Example:** School email → fake sign-in message → someone reads school messages → use MFA and report unexpected sign-in prompts.

**Check:** The learner can tell the difference between an asset, a threat and a control.

### Practical 2 — Apply the CIA triad to a file

**You need:** a new practice document on your own device.

1. Open Notepad, Text Editor or another basic writing app.
2. Type a made-up class note, such as “Science revision: plants need light and water.” Do not include personal details.
3. Save it in a folder named `Cybersecurity Practice`.
4. Discuss: who should be able to read it (confidentiality)? How would you notice an unwanted edit (integrity)? How could you get it back if deleted (availability)?
5. Choose one protection for each answer: restricted access, a review/copy, and a backup.

**Check:** Learner gives one everyday example for each CIA word.

## Day 2 — Computers, operating systems and files

### Practical 3 — Find your computer's basic information

**You need:** your own computer. Do not change settings.

1. On Windows, open **Settings → System → About**. On Ubuntu/Linux, open **Settings → About** (or use `hostnamectl` in Terminal).
2. Note the operating system name and version and the device name. Do not share a serial number publicly.
3. Open the task manager: press `Ctrl+Shift+Esc` on Windows, or open **System Monitor** on Linux.
4. Find one running application and one background process. Do not end either process.
5. Explain the difference: an application is what you opened; a process is a program currently running.

**Check:** Learner can locate the OS version and describe one running process.

### Practical 4 — Review a file and account safely

1. In File Explorer or Files, open the practice folder from Practical 2.
2. Find the file name, file type/extension and last-modified date. Do not open unknown files.
3. On Windows, open **Settings → Accounts** and identify whether the signed-in account is standard or administrator if shown. On Linux, open **Settings → Users** and view your account type; do not change it.
4. Open **Settings → Windows Update** or **Software Updater** and check whether updates are offered. Do not interrupt an update already in progress; ask the trainer before installing on a shared device.
5. Record one safe observation and one question for the trainer.

**Check:** Learner can describe why administrator access should be limited and updates matter.

## Day 3 — Networking fundamentals

### Practical 5 — Trace your own network connection

1. Connect to your home or classroom network with permission.
2. On Windows, open Command Prompt and type `ipconfig`. On Linux, open Terminal and type `ip addr`.
3. Find the connected network interface and its local IP address. Do not post this information publicly.
4. On Windows, type `ipconfig` and find **Default Gateway**. On Linux, type `ip route` and find the line marked `default`.
5. Draw: `This computer → Wi-Fi router → Internet`. Label the computer's address and router as the gateway.

**Check:** Learner can explain that a local IP address helps identify a device on its network.

### Practical 6 — Check connectivity and name lookup

1. Open Command Prompt or Terminal.
2. Type `ping 127.0.0.1`. This tests the computer's own network software, not another person's device.
3. Type `nslookup example.com` (Windows/Linux) or `dig example.com` if `dig` is installed.
4. Note whether the name lookup returned an address. A blocked response does not automatically mean something is broken; school networks may restrict tools.
5. Close the window and write what each check tested: local network software versus looking up a website name.

**Check:** Learner can explain that DNS looks up names and that one failed test is not proof of an attack.

## Day 4 — Linux command line

### Practical 7 — Navigate Linux without changing the system

**You need:** a Linux computer or instructor-provided Linux virtual machine. Do not use `sudo`.

1. Open **Terminal** from the applications menu.
2. Type `whoami` and press Enter to see the current username.
3. Type `pwd` to see the current folder.
4. Type `ls` to list items in that folder, then `cd Documents` if that folder exists, followed by `pwd` again.
5. Type `cd` to return to your home folder. Write down what each command showed.

**Check:** Learner uses `whoami`, `pwd`, `ls` and `cd` correctly.

### Practical 8 — Create and search a practice note in Linux

1. In Terminal, type `mkdir -p ~/Cybersecurity-Practice`.
2. Type `printf 'class practice: report suspicious messages\n' > ~/Cybersecurity-Practice/notes.txt`.
3. Type `cat ~/Cybersecurity-Practice/notes.txt` to display the note.
4. Type `grep 'suspicious' ~/Cybersecurity-Practice/notes.txt` to find the word.
5. Type `ls -l ~/Cybersecurity-Practice/notes.txt` and observe the file permissions. Do not change them.

**Check:** Learner can explain that `>` writes the practice note and `grep` searches its text.

## Day 5 — Cyber threats and safe reporting

### Practical 9 — Spot warning signs in a sample message

**You need:** an instructor-provided screenshot or printed fake message. Do not search for or open a real suspicious message.

1. Read the message without clicking anything.
2. Check the sender name and address, unexpected urgency, spelling, link text, attachment and requested action.
3. Use **SULAR-V**: Sender, Urgency, Link, Attachment, Request, Verify.
4. Mark each clue as “present,” “not present” or “not enough information.”
5. Write the safe next step: use a separate trusted contact method to verify, then report it.

**Check:** Learner explains why a familiar display name is not proof of identity.

### Practical 10 — Write a safe reporting message

1. Open a blank practice document.
2. Write the date/time of the simulated message, the channel where it arrived and what it asked the recipient to do.
3. Describe suspicious clues without copying or opening the link or file.
4. Add the action taken: “I did not click. I verified using a known contact method. I reported it to [teacher/IT contact].”
5. Read the report aloud to a partner and check that it is factual, calm and does not include a password.

**Week 1 result:** each learner submits an asset map, a basic network drawing, Linux command notes and a phishing report.

---

# Week 2 — Protection and Defense
## Days 6–10: Protect accounts, devices and networks

**Phase:** Protection and Defense  
**Duration:** 5 training days / 25 contact hours  
**Audience:** Beginners who completed Week 1  
**Approach:** Demonstration • Safe configuration review • Guided lab

> **Week 2 theme:** Protect accounts and devices, then learn how defenders observe network activity.

## Week 2 learner outcomes

By the end of Week 2, learners should be able to:
1. Explain identification, authentication and authorization.
2. Apply unique passphrases, MFA and least-privilege thinking.
3. Locate endpoint, update and firewall protection settings without disabling them.
4. Describe basic network segmentation, Wi-Fi security and VPN purpose.
5. Read instructor-provided packet evidence and follow written test scope.

### Week overview

By Friday, learners should be able to improve the safety of their own accounts, review basic device protections, describe a safer Wi-Fi setup, read a prepared packet capture and explain what authorized security testing means.

### Core lesson

**Identity and access management** is about knowing who is signing in and what that person is allowed to do. Identification names the account, authentication checks proof of identity, and authorization decides what the account can do. A passphrase should be long and unique. MFA combines different factor types, such as something you know (a password), something you have (a registered device), or something you are (a biometric). Two passwords are not two different factor types. A password manager can help keep different passwords. **Least privilege** means a person gets only the access needed for their role; **role-based access** groups permissions by job.

Devices need updates, antivirus/endpoint protection, a firewall and safe account settings. A network firewall controls traffic between networks; a host firewall protects one computer. Wi-Fi should use modern security, a strong router-admin password and a separate guest network. A VPN creates an encrypted connection to a trusted VPN service or organization; it does not make every online activity anonymous or automatically safe.

Wireshark displays network packets. A packet capture can contain private information, so use only a trainer-provided sanitized sample. A security test must have permission and a precise scope. Learning to observe and report is enough; learners should not exploit weaknesses.

### Everyday example

A classroom has a teacher, learners and visitors. If everyone uses the same key, it is hard to know who entered and visitors might reach staff rooms. Individual accounts, role-based permissions and a guest network work like separate keys for separate needs.

### Live scenario — “A shared account after a staff change”

A former employee still knows a shared office password. Ask what could go wrong and what the organization should do. Good answers include disabling the old account, changing shared secrets, reviewing access, enabling MFA and keeping an owner for each account. Do not ask learners to try the old password.

### Five-day plan

| Day | Lesson | Practical numbers |
|---|---|---|
| 6 | Passwords, MFA and access control | 1–2 |
| 7 | Windows endpoint security | 3–4 |
| 8 | Firewalls, Wi-Fi and VPNs | 5–6 |
| 9 | Packet analysis | 7–8 |
| 10 | Authorized security testing | 9–10 |

## Day 6 — Identity, passwords and access control

### Practical 1 — Improve one account's sign-in safety

**Use:** your own account or a trainer-provided practice account. Never tell the class your password or MFA code.

1. Open the account's official settings by typing its known address yourself or using its official app.
2. Find **Security**, **Sign-in** or **Two-step verification**.
3. If allowed, turn on MFA and follow the service's official setup prompts. If not, write down where the setting is and ask the account owner.
4. Save recovery information in a safe place that is not shared with the class. Do not use a classmate's phone or account as your recovery method.
5. Check for sign-in alerts and sign out of the practice session when finished.

**Check:** Learner can name two independent sign-in factors without revealing either one.

### Practical 2 — Make a role-and-access table

1. Create a table with three pretend roles: learner, teacher and IT administrator.
2. Add resources: class notes, grades, staff payroll and Wi-Fi settings.
3. For each role/resource pair, write “view,” “edit” or “no access.”
4. Give each person only the access needed for the job. For example, learners may view their own grades but not payroll.
5. Add a row for “person leaves the organization”: the account owner should disable access and review shared access.

**Check:** Learner can explain least privilege and why shared accounts make accountability difficult.

## Day 7 — Windows endpoint security

### Practical 3 — Review Windows protection status

1. Open **Start → Windows Security**.
2. Select **Virus & threat protection** and note whether protection appears on or needs attention.
3. Select **Firewall & network protection** and view the active network profile.
4. Check **App & browser control** for any visible warning or status.
5. Do not switch off a control or change a warning setting. Record the result and show the trainer if something says “action needed.”

**Linux option:** open the installed security/update settings and review status with the trainer. Do not install or remove firewall software during this exercise.

**Check:** Learner can locate protections and report status without disabling them.

### Practical 4 — Check update and sign-in settings

1. On Windows, open **Settings → Windows Update**. On Linux, open **Software Updater** or the system's update page.
2. Note whether the system says it is up to date or offers updates.
3. Open **Settings → Accounts → Sign-in options** (Windows) or **Settings → Users** (Linux).
4. Confirm that the device uses a screen lock or password. Do not change another person's settings.
5. Write one reason updates and screen locks help. Ask the owner/trainer before installing updates on a shared classroom device.

**Check:** Learner can describe how updates fix known problems and screen locks limit casual access.

## Day 8 — Network security, Wi-Fi and VPNs

### Practical 5 — Draw a safer small-office network

1. Draw a box for the internet and connect it to a router/firewall.
2. Add a staff network with work computers and a separate guest Wi-Fi network.
3. Add a server only if the office needs one; label who should access it.
4. Show that guest Wi-Fi should not reach staff devices or the server.
5. Add a note: WPA2/WPA3, strong router-admin password, updates and MFA for remote access.

**Check:** Learner can explain why guest and staff access should be separated.

### Practical 6 — Review the Wi-Fi settings without changing them

1. Ask permission before opening the home or classroom router settings. If permission is unavailable, use the trainer's screenshots.
2. Find the Wi-Fi security mode and identify whether it says WPA2 or WPA3. Do not record or share the Wi-Fi password.
3. Find the router administration page and check whether the default admin password has been changed; do not attempt to sign in if you do not own/manage it.
4. Look for a guest-network option and note whether guest access is separate.
5. Give the owner a short recommendation list; do not change router settings in class.

**Check:** Learner distinguishes a Wi-Fi password from the router administrator password.

## Day 9 — Packet analysis with Wireshark

### Practical 7 — Read a prepared packet capture

**You need:** Wireshark and a sanitized capture supplied by the trainer. Do not capture shared Wi-Fi or other people's traffic.

1. Open Wireshark and choose **File → Open** to load the trainer's `.pcap` or `.pcapng` sample.
2. Click a packet and find the source, destination and protocol columns.
3. In the display-filter box, type `dns` and press Enter.
4. Select a DNS packet and identify the requested name in the details pane. Do not follow links or contact the address.
5. Clear the filter and write one sentence describing what a DNS request does.

**Check:** Learner can tell source, destination and protocol apart.

### Practical 8 — Compare DNS and HTTPS observations

**Use the same trainer-provided capture.**

1. Type `dns` in Wireshark's display-filter box and observe a name lookup.
2. Replace the filter with `tls` or `tcp.port == 443` and observe a secure web connection if the sample contains one.
3. Compare what is visible: DNS may show the requested name; encrypted web content should not appear as ordinary readable page text.
4. Record the source, destination and protocol for one example of each.
5. Explain why encryption helps protect data in transit but does not prove that a website is trustworthy.

**Check:** Learner avoids claiming that HTTPS means a site is honest or harmless.

## Day 10 — Ethical security testing and scope

### Practical 9 — Write rules of engagement for a tiny lab

1. Name one computer that the instructor owns or has explicitly approved as the practice target.
2. Write the exact target, activity, date/time and person supervising it.
3. List what is not allowed: other devices, other networks, password guessing, exploitation or data changes.
4. Write how to stop the exercise and who to contact if anything unexpected happens.
5. Ask the trainer to approve the scope before using any discovery tool.

**Check:** Learner understands that “it is online” does not mean “I have permission.”

### Practical 10 — Observe only your own computer

**Optional, trainer-supervised command exercise. Run only against `127.0.0.1`, your own computer.** If Nmap is not already installed, do not install it for this class; complete the worksheet instead.

1. Confirm with the trainer that the target is exactly `127.0.0.1` (your own computer).
2. Open Terminal or Command Prompt on your own device.
3. If Nmap is already installed, type `nmap 127.0.0.1` and wait for it to finish. Do not add other addresses or options.
4. Record only the ports the tool reports as open, if any. “No open ports” is a valid result.
5. Close the terminal and explain that the observation is limited to the approved local computer.

**Alternative:** interpret an instructor-provided sample scan report and recommend one safe follow-up question.

**Week 2 result:** each learner submits an access table, a network diagram, packet observations and an approved-scope worksheet.

---

# Week 3 — Detection and Application Security
## Days 11–15: Find weaknesses, protect data and review evidence

**Phase:** Detection and Application Security  
**Duration:** 5 training days / 25 contact hours  
**Audience:** Beginners who completed Weeks 1–2  
**Approach:** Sample-based investigation • Defensive review • Clear reporting

> **Week 3 theme:** Identify meaningful weaknesses, protect information and interpret evidence carefully.

## Week 3 learner outcomes

By the end of Week 3, learners should be able to:
1. Describe the vulnerability-management cycle and prioritize a sample finding.
2. Explain basic web requests, responses, sessions and access-control risks.
3. Distinguish encryption, hashing and encoding.
4. Review account, cloud-sharing and email-security settings responsibly.
5. Read a simple log and create a fact-based alert-triage note.

### Week overview

By Friday, learners should be able to prioritize a simple security weakness, recognize common web concepts, check a file's hash, review safe cloud sharing settings and explain what a basic security alert means.

### Core lesson

Vulnerability management is a repeating process: find a possible weakness, validate it, prioritize it, remediate it, then verify the fix. A CVE is an identifier for a publicly disclosed vulnerability; a severity score describes technical characteristics, not the full business risk. Consider whether the system is exposed, how important the asset is, whether a fix exists and what harm is plausible. Record uncertainty and possible false positives rather than presenting an unverified scanner result as fact.

A web browser sends a request to a web server and receives a response. URLs identify locations; HTTP methods describe actions; status codes describe results. Cookies can help a site remember a session. Input validation checks whether submitted information is in the expected form. Broken access control means someone can reach information or actions they should not.

**Encryption** protects information so it can be read with the right key. **Hashing** creates a fixed-length fingerprint used to compare data. **Encoding** changes a representation and is not a secret protection. Cloud providers and customers share security responsibilities. Logs record events; monitoring looks for patterns that may need investigation.

### Everyday example

A school stores a class list in a cloud folder. If “anyone with the link” can view it, the risk is unnecessary exposure. Use a private dummy file to practise, share it only with named test accounts, then remove the sharing link.

### Live scenario — “A strange sign-in alert”

A teacher sees an alert for a sign-in from an unfamiliar place. Ask what is known, what is only assumed and what safe checks come next. The teacher should use the service's official sign-in page, review recent account activity, change the password if the provider or IT team advises, revoke unknown sessions and report the alert. Do not click a link in an unexpected alert.

### Five-day plan

| Day | Lesson | Practical numbers |
|---|---|---|
| 11 | Vulnerability management and risk | 1–2 |
| 12 | Web and application security | 3–4 |
| 13 | Cryptography and data protection | 5–6 |
| 14 | Cloud, email and online services | 7–8 |
| 15 | Monitoring, logs and SOC basics | 9–10 |

## Day 11 — Vulnerability management and risk

### Practical 1 — Prioritize a sample weakness

**You need:** this made-up finding: “The public school website is running old software. The site contains a public timetable, but no student records.”

1. Write down the asset: the public school website.
2. Write the weakness: old software that may contain known security problems.
3. Rate likelihood from 1 (unlikely) to 3 (likely) and impact from 1 (small) to 3 (serious). Explain your choices; there is no exact score expected.
4. Multiply the numbers for a simple priority score, then note why a real team would need more evidence.
5. Recommend a safe next step: owner confirms the software and plans an update using the approved process.

**Check:** Learner explains that a score helps organize work but is not proof of compromise.

### Practical 2 — Read an instructor-provided scan report

**Do not scan a real website. Use only the report supplied by the trainer.**

1. Find the asset name and scan date in the report.
2. Find one finding and copy its title, severity and evidence into a worksheet.
3. Mark each statement as a fact from the report or an assumption.
4. Write one question needed to validate the finding, such as “Is this service reachable from the internet?”
5. Write a remediation recommendation for the system owner, then state how the team could verify it was fixed.

**Check:** Learner does not try to exploit or retest a system outside the approved scope.

## Day 12 — Web and application security

### Practical 3 — Inspect a safe web page in the browser

1. Open a familiar, trusted website by typing its known address. Do not log in or enter personal details for this exercise.
2. Point to the address bar and identify `https` and the site name.
3. Open browser developer tools: press `F12` or right-click the page and choose **Inspect**.
4. Select **Network**, reload the page, and click one request. Find its method and status code if visible.
5. Close developer tools. Write what a request and response are in your own words. Do not change or replay requests.

**Check:** Learner knows that seeing HTTPS alone does not establish that a site is legitimate.

### Practical 4 — Review a safe web-app example

**Use:** a trainer-provided screenshot, worksheet or intentionally vulnerable training app hosted in the course lab. Do not test a public site.

1. Identify the sign-in page, a user input box and the page that should be private.
2. For each, ask: “Who should be allowed to see or change this?”
3. Review the supplied example of a weak access rule or unsafe input. Do not enter attack strings or attempt to bypass it.
4. Describe the problem in plain language, such as “A learner should not be able to view another learner's record.”
5. Recommend checking the user's permission on the server and safely validating input. Give the note to the trainer.

**Check:** Learner can describe the risk and a defensive fix without attempting exploitation.

## Day 13 — Cryptography and data protection

### Practical 5 — Compare file hashes

1. Create a practice text file named `hash-practice.txt` containing `Cybersecurity class sample`.
2. On Windows, open PowerShell in the folder and run `Get-FileHash .\hash-practice.txt -Algorithm SHA256`. On Linux, open Terminal in the folder and run `sha256sum hash-practice.txt`.
3. Copy the hash into your worksheet. Do not treat the hash as a password.
4. Change one character in the file, save it, and calculate the hash again.
5. Compare the two values. Explain that a changed hash indicates the file contents changed, but does not tell you who changed them.

**Check:** Learner can distinguish a hash from encryption.

### Practical 6 — Protect a practice file

1. Create a document containing made-up information only, such as a pretend event plan.
2. Save it inside a clearly named practice folder on your own device.
3. Make a second copy in a separate practice folder or instructor-approved backup location.
4. Review who can access the folder using the system's sharing/permissions page; do not grant access to other people during class.
5. Write which protection addresses access, which addresses accidental loss and why secure deletion matters for real sensitive data.

**Check:** Learner names one protection for data at rest and one for data availability.

## Day 14 — Cloud, email and online service security

### Practical 7 — Safely review cloud sharing

**Use:** a practice account or a personal account with a dummy file only. Do not upload real personal or school records.

1. Create a file that says `Practice document - no personal information`.
2. Open the service's sharing settings and check whether access is private, named people only or anyone with a link.
3. Keep the file private. If it is already shared, remove unneeded access only if you own the file; otherwise ask the owner.
4. Find the setting for download, expiry or link access if available; do not change organization-owned settings.
5. Delete the dummy file or leave it private, then write what the service owner protects and what the user must protect.

**Check:** Learner can describe shared responsibility and identify an overly broad link.

### Practical 8 — Review account and email security options

1. Open the official settings page of your own email or practice account.
2. Locate MFA, recovery options, recent sign-ins and forwarding rules. Do not share the screen if private details are visible.
3. Check whether you recognize the recovery method and recent sign-ins; do not remove anything you do not understand.
4. If a forwarding rule looks unfamiliar, take a screenshot only if allowed and report it to the account owner/support team.
5. Sign out of the practice session and write one improvement to discuss with the trainer.

**Check:** Learner knows to investigate unfamiliar account changes via the official provider or IT team.

## Day 15 — Security monitoring, logs and SOC basics

### Practical 9 — Read a simple security log

**Sample data:** `09:00, Amina, successful sign-in, classroom PC`; `09:04, Amina, failed sign-in, classroom PC`; `09:05, Amina, failed sign-in, classroom PC`; `09:06, Amina, successful sign-in, classroom PC`.

1. Copy the sample rows into a spreadsheet or table in a document.
2. Label the columns: time, user, event and device.
3. Circle the failed sign-ins and note how many occurred.
4. Write what you know (three failed attempts followed by success) and what you do not know (who typed them or whether the user made a mistake).
5. Write a safe follow-up: confirm with the user or account owner and check the relevant official account/device logs.

**Check:** Learner separates observed evidence from a guess about cause.

### Practical 10 — Perform a mini alert triage

1. Read this trainer scenario: “An account had several failed sign-ins, then a successful sign-in. The owner says they were signing in from the classroom.”
2. Record **what, when, where, who** using only the facts supplied.
3. Choose a priority: low, medium or high, and explain the reason. Escalate if the sign-in was not recognized or sensitive access is involved.
4. List two safe next checks, such as account activity and endpoint alerts, performed by the authorized owner/IT team.
5. Write a two-sentence ticket update: facts, action taken and next owner.

**Week 3 result:** each learner submits a risk note, web observation, hash comparison, cloud-sharing review and alert-triage ticket.

---

# Week 4 — Response, Governance and Career Readiness
## Days 16–20: Respond carefully, preserve evidence and communicate

**Phase:** Response, Governance and Career Readiness  
**Duration:** 5 training days / 25 contact hours  
**Audience:** Beginners who completed Weeks 1–3  
**Approach:** Tabletop scenarios • Evidence handling • Team capstone

> **Week 4 theme:** Respond calmly, preserve reliable evidence and communicate useful next steps.

## Week 4 learner outcomes

By the end of Week 4, learners should be able to:
1. Describe incident-response stages and know when to escalate.
2. Record an incident timeline and preserve trainer-provided evidence.
3. Explain hashes, chain of custody and basic privacy responsibilities.
4. Draft a simple acceptable-use rule and risk register.
5. Present a concise, evidence-based incident summary to a technical or non-technical audience.

### Week overview

By Friday, learners should be able to describe a basic incident response, preserve simple evidence without changing it, write a small-organization policy, explain a risk clearly and present a beginner-level capstone report.

### Core lesson

Incident response is a planned way to handle a security problem: prepare, detect and analyze, contain, eradicate the cause, recover and learn. In a real incident, follow the organization's plan and contact the responsible IT/security person. A beginner should not delete files, confront a suspected person, or independently shut down a business system. Escalate quickly when there may be exposure of personal data, financial systems or safety-critical services.

Digital forensics examines digital evidence. A hash can help check whether a file changed between two points in time, but cannot identify who changed it or prove that it is true. A chain-of-custody record says who handled evidence, when, where and why. Keep the original unchanged; work on an authorized copy. A policy explains expected rules; a procedure gives steps. Risk management weighs likelihood and impact, records existing controls and residual risk, and names the person who owns the decision.

Security operations teams monitor alerts, record tickets, gather evidence, escalate and communicate. A useful report gives the issue, evidence, impact, action, owner and next step. Technical findings should be understandable to non-technical people too.

### Everyday example

If a school laptop is reported missing, the first response is not to guess who took it. Record when it was last seen, tell the responsible staff member, protect accounts that may have been signed in, preserve available records and follow the school's incident procedure.

### Live scenario — “A learner reports a suspicious file”

A learner says a computer displayed a warning after an unexpected download. Ask what to do first. Safe answers: stop interacting with the file, do not forward or delete it, note the time and exact warning, tell the trainer/IT contact, and follow their containment instructions. Use a prepared screenshot in class; do not create malware or reproduce the event.

### Five-day plan

| Day | Lesson | Practical numbers |
|---|---|---|
| 16 | Incident response and containment | 1–2 |
| 17 | Forensics and evidence | 3–4 |
| 18 | Governance, risk and privacy | 5–6 |
| 19 | Security operations and careers | 7–8 |
| 20 | Integrated capstone | 9–10 |

## Day 16 — Incident response and containment

### Practical 1 — Walk through an incident response

**Scenario:** A staff member reports an unexpected sign-in alert. No one knows yet whether the account was accessed by someone else.

1. Write **Prepare**: who is the IT contact and where is the reporting channel?
2. Write **Detect/Analyze**: what exactly did the alert say, and when did it arrive?
3. Write **Contain**: the authorized account owner/IT team may revoke unknown sessions or temporarily restrict the account; do not do this to someone else's account.
4. Write **Eradicate/Recover**: follow the provider/IT team's process to secure the account and restore normal access.
5. Write **Learn**: what control or training might reduce recurrence?

**Check:** Learner knows to report promptly and not independently alter another person's account.

### Practical 2 — Create a simple incident record

1. Open a new practice document and give the case a made-up ID, such as `CLASS-001`.
2. Record the reported time, device/account involved and who reported it (use pretend names).
3. Separate **observed facts** from **unconfirmed ideas**.
4. Record who was notified and what safe action was taken; do not include passwords or MFA codes.
5. Add the next action, the person responsible and a time to review it.

**Check:** A different learner can read the note and understand what happened without guessing.

## Day 17 — Digital forensics and evidence

### Practical 3 — Inventory evidence without changing it

**Use:** a trainer-provided screenshot, sample log or dummy file only.

1. Make a table with evidence ID, description, source, collection time and collector.
2. Give the item an ID such as `E-01`; describe it without making a claim about guilt or cause.
3. Record where the trainer says it came from and who supplied it.
4. Do not rename, edit, delete, forward or upload the original item.
5. Ask the trainer where an authorized working copy should be stored.

**Check:** Learner explains why evidence should be preserved and handled consistently.

### Practical 4 — Calculate a practice-file hash

1. Create a dummy file named `evidence-sample.txt` containing `Practice evidence only`.
2. On Windows, open PowerShell in that folder and run `Get-FileHash .\evidence-sample.txt -Algorithm SHA256`. On Linux, run `sha256sum evidence-sample.txt` from Terminal in that folder.
3. Record the filename, hash, date/time and tool used in your evidence table.
4. Make a copy of the file and calculate the copy's hash. Confirm the values match.
5. Change one character in the copy and calculate its hash again. Record that the changed value indicates changed contents.

**Check:** Learner describes a hash as a comparison fingerprint, not proof of who created a file.

## Day 18 — Governance, risk and privacy

### Practical 5 — Draft a one-page acceptable-use rule

1. Create a document titled **Safe Use of School Devices**.
2. Write who the rule applies to: learners, staff and approved visitors.
3. Add five plain-language rules: use your own account, lock the screen, install only approved apps, report suspicious messages, and keep school information private.
4. Add one reporting contact role, such as “teacher or IT support”; do not invent a real person's contact details.
5. Ask a partner to read it and mark any words a beginner may not understand; replace those words with simpler ones.

**Check:** The policy says what to do and who it applies to, in language learners understand.

### Practical 6 — Make a small risk register

1. Create columns for asset, risk, likelihood (1–3), impact (1–3), control, owner and review date.
2. Add a fictional school email account as the first asset.
3. Enter a risk such as “someone reuses a password from another site.”
4. Choose likelihood and impact scores and multiply them to get a simple priority number.
5. Add controls such as unique passphrases, MFA and an account owner; set a review date.

**Check:** Learner can explain that scores help prioritize discussion and are not exact predictions.

## Day 19 — Security operations and career readiness

### Practical 7 — Triage an alert like a SOC analyst

**Sample alert:** “Two failed logins for `student-demo`, then one success at 10:15 from the classroom computer.”

1. Create a ticket with a made-up ID and copy the alert exactly.
2. Write what happened, when, where and which account/device were involved.
3. List one normal explanation and one concerning explanation without deciding which is true.
4. Assign an initial priority and explain what would raise it, such as an unrecognized sign-in or access to sensitive records.
5. State the safe escalation: send the ticket to the authorized account owner/IT team and wait for instructions.

**Check:** Learner does not label the event an attack based on one clue alone.

### Practical 8 — Build a beginner cybersecurity portfolio page

1. Open a word processor or a new local document.
2. Add your name (or a class alias), the course skills practised and tools used.
3. Include one sanitized sample: a network diagram, a fictional risk register or an incident report with all personal details removed.
4. Add a short explanation of what you did, what you learned and what you would improve.
5. Save locally as `Cybersecurity-Portfolio-Practice`. Do not publish account details, internal school information, real logs or confidential findings.

**Check:** Portfolio shows clear communication and responsible handling of information.

## Day 20 — Integrated cybersecurity capstone

### Practical 9 — Capstone team investigation

**Trainer prepares:** a fictional case pack with a suspicious-email screenshot, a short login log, a sanitized packet capture or summary, a basic endpoint alert and a pretend asset list. Do not use live attacks or real account data.

1. Assign team roles: coordinator, evidence recorder, risk reviewer and presenter. Small teams may combine roles.
2. Read the case pack and create a timeline. Record facts separately from assumptions.
3. Identify affected assets, possible risks and the evidence that supports each concern.
4. Recommend immediate safe actions for the authorized IT owner, followed by recovery and prevention steps.
5. Prepare a one-page incident summary with issue, evidence, impact, action, owner and next step.

**Check:** Every recommendation is linked to a fact or clearly marked as something to verify.

### Practical 10 — Present and review the capstone

1. Present the team's one-page summary in five minutes using plain language.
2. Explain one key finding, what evidence supports it and one thing that remains uncertain.
3. Give two prioritized recommendations and identify who should own each action.
4. Answer questions without sharing secrets or claiming more than the evidence shows.
5. Complete an individual reflection: one skill learned, one safety rule remembered and one topic to keep practising.

**Week 4 result:** each learner contributes to an incident record, evidence worksheet, risk register, portfolio sample and capstone presentation.

---

# Instructor Wrap-Up

## End-of-course learner checklist

- [ ] I can explain assets, threats, vulnerabilities, risks and controls.
- [ ] I can use basic computer and network information screens safely.
- [ ] I can explain passwords, MFA, least privilege and updates.
- [ ] I can recognize common phishing warning signs and report them safely.
- [ ] I understand that security testing needs clear permission and scope.
- [ ] I can describe what a log, alert, hash and incident record are for.
- [ ] I can recommend a practical control and explain it in plain language.
- [ ] I know when to stop and ask the responsible trainer or IT person.

## Simple assessment guide

For each practical, assess whether the learner followed the steps safely, recorded what they observed, distinguished facts from assumptions and could explain the result in their own words. Reward careful reporting and safe decisions, not just fast tool use.

## Closing message for learners

Good cybersecurity starts with curiosity and care: understand what you are protecting, get permission, observe carefully, preserve evidence, and explain what you found clearly.