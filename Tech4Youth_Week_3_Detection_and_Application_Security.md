# Cybersecurity Training
## Beginner Lecture Notes and Step-by-Step Practicals

**Duration:** 5 training days / 25 contact hours

Use this weekly guide alongside the instructor. Follow each practical in order, use made-up data where requested, and ask the trainer before changing settings. Work only on your own device, a device you have permission to use, or an instructor-provided lab. Never test public systems or other people’s accounts. Do not share passwords or MFA codes.

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

