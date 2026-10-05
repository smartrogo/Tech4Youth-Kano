# Cybersecurity Training
## Beginner Lecture Notes and Step-by-Step Practicals

**Duration:** 5 training days / 25 contact hours

Use this weekly guide alongside the instructor. Follow each practical in order, use made-up data where requested, and ask the trainer before changing settings. Work only on your own device, a device you have permission to use, or an instructor-provided lab. Never test public systems or other people’s accounts. Do not share passwords or MFA codes.

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

