# Cybersecurity Training
## Beginner Lecture Notes and Step-by-Step Practicals

**Duration:** 5 training days / 25 contact hours

Use this weekly guide alongside the instructor. Follow each practical in order, use made-up data where requested, and ask the trainer before changing settings. Work only on your own device, a device you have permission to use, or an instructor-provided lab. Never test public systems or other people’s accounts. Do not share passwords or MFA codes.

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

