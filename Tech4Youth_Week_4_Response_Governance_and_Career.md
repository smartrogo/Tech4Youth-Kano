# Cybersecurity Training
## Beginner Lecture Notes and Step-by-Step Practicals

**Duration:** 5 training days / 25 contact hours

Use this weekly guide alongside the instructor. Follow each practical in order, use made-up data where requested, and ask the trainer before changing settings. Work only on your own device, a device you have permission to use, or an instructor-provided lab. Never test public systems or other people’s accounts. Do not share passwords or MFA codes.

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
