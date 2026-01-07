# Onboarding Plan for Software Development Tasks

> Standup meeting 11:00 [Meeting Link](DD_LINK_HERE)

---

## 1. 📅 Work From Home (WFH) - Work From Office (WFO) Alignment

- Every member must be **available at the office at least 12 days per month**.  
- Notify on Slack if you plan to work from home **the day before**.  
- At the end of each day, submit your request **after completing your timesheet**, and attach a snapshot of your timesheet in the request.  
- The timesheet should **contain evidence of work done**, including a brief description of your activity if your ticket is not yet finished.  
- If additional work is needed, **update the ticket with a patch of code or relevant progress**.  
- To ensure everyone completes the **minimum 12 WFO days**, requests will only be approved **at the end of the month** or when each member meets their WFO requirement.  
- **Vacation days are not deducted** from office days.  

[View Excel Tracking Sheet](ADD_EXCEL_SHEET_LINK_HERE)


---

## 2. 🕓 Support & Escalation Model

- Support is actively monitored during the hours listed below. Outside these hours, response times may be slower. we should align expectations accordingly.

### Support Rules
- Developers should escalate **after 15–30 minutes of blockage**.  
- Issues must include:
  - Problem description  
  - Steps attempted  
  - Error messages/logs  

### Available Time
- I will be available for support for **1.5 → 2 hours per day**:  
  - **11:30 AM – 12:00 PM**  
  - **4:30 PM – 5:00 PM**  
- Outside these hours, send a message and I will respond according to the **Response SLAs**.

### Response SLAs
- **Office days:** 5–10 minutes  
- **WFH days:** ≤ 15 minutes  

### Escalation Path
1. Developer → Team Lead  
2. Team Lead → Other Lead  
3. Team Lead → Team Manager (if delivery is at risk)  
4. If Team Lead is unavailable → Team Manager  
5. If you provide support for a colleague, **record this in Generic ticket** with the title **"Team Support"**.

---

## 3. 🗓️ Weekly One-on-One Meetings

- I will hold **weekly one-on-one meetings** with each team member.  
- **Duration:** Maximum **15–30 minutes** per meeting.  
- **Purpose:**  
  - Review progress from the previous week.  
  - Discuss blockers or challenges.  
  - Align priorities for the upcoming week.  
- Meetings will be scheduled individually, and team members should **come prepared with updates and questions**.  
- Notes and action items from these meetings will be tracked for follow-up in the next session.  

---

# 📋 Estimation Examples for Software Development Tasks

> These assume reasonable familiarity with the codebase. New developers should apply a **+50% time buffer** and escalate if progress stalls or estimates are exceeded.

---

## 🖼️ Frontend Tasks

| Task | Estimated Time | Escalation Time | Notes |
|------|----------------|----------------|-------|
| Fix UI alignment or spacing | 1 hour | 2 hours | Simple CSS/layout adjustment |
| Add form validation rule | 2 hours | 3 hours | Using existing form & validation logic |
| Create new static page (no logic) | 1 day | 1.5 days | Simple page with design & text |
| Create interactive form with validation | 1.5 days | 2.5 days | Includes controlled components |
| Integrate new API into frontend | 1–2 days | 3 days | Depends on API readiness & UI complexity |
| Refactor reusable component | 2–3 hours | 5 hours | Small-scale component extraction or cleanup |

---

## ⚙️ Backend Tasks

| Task | Estimated Time | Escalation Time | Notes |
|------|----------------|----------------|-------|
| Fix a null pointer or exception | 1–2 hours | 3 hours | If root cause is known |
| Add a new endpoint (GET/POST) | 1 day | 1.5 days | Assuming models/services mostly exist |
| Add DB migration script | 2–4 hours | 6 hours | Simple table/column addition |
| Update existing service logic | 0.5–1 day | 1 day | If logic is well understood |
| Implement business rule | 1.5–2 days | 3 days | Moderate complexity |
| Integrate with external API | 2–3 days | 4 days | Requires auth, error handling, retries |

---

## 🔁 Full-Stack / Integration

| Task | Estimated Time | Escalation Time | Notes |
|------|----------------|----------------|-------|
| Add backend + frontend for new dropdown | 1 day | 1.5 days | DB lookup + form integration |
| Create new list + detail view | 2–3 days | 4 days | CRUD, filters, pagination |
| Build simple dashboard widget | 1.5 days | 2.5 days | Includes UI + backend metrics |
| Refactor feature across layers | 3–5 days | 1 week | Includes testing, regression check |

---

## 🧪 Testing

| Task | Estimated Time | Escalation Time | Notes |
|------|----------------|----------------|-------|
| Manual verification of bug fix | 0.5–1 hour | 2 hours | Includes environment setup |

---

## 🗃️ Environment

| Task | Estimated Time | Escalation Time | Notes |
|------|----------------|----------------|-------|
| Debug environment config issue | 2–3 hours | 5 hours | Depends on logs/debugging tools |

---

## 🟨 Notes for New Developers

- ✅ Use these examples as a **starting point**.  
- 📈 Apply **+50% time buffer**.  
- 🚩 Raise a flag if:
  - Blocked for ≥ 30 minutes  
  - You reach 50% of estimated time with <50% task completion  
  - Scope or complexity changes mid-way

---

# 🔧 Support Ticket Priority & SLA – Detailed Breakdown

| Priority | Impact & Description | Examples | Developer Response Time | Expected Resolution Time | Escalation Policy | Communication |
|----------|--------------------|---------|------------------------|------------------------|-----------------|---------------|
| **P0 – Critical / Blocker** | Complete system outage or critical feature broken; blocks testing, releases, or business operations | API down, service crash, production outage, data loss risk | Within 30 minutes | Within 2 hours | Immediate escalation to senior dev, team lead & on-call | Continuous updates every 30 min until resolved |
| **P1 – High** | Major functionality impaired; blocks important workflows | Login failure, gateway error, broken key API | Within 1 hour | Within 4–8 hours | Escalate to senior dev if unresolved after 8 hours | Updates every 1–2 hours |
| **P2 – Medium** | Partial functionality impacted; workaround available | UI misalignment, incorrect data display, intermittent API errors | Within 4 hours | Within 1–2 business days | Escalate to senior dev if unresolved after 2 days | Daily updates |
| **P3 – Low** | Minor bugs, general questions, documentation requests | Typos, UI color mismatch, request for enhanced logs | By next business day | Within 3–5 business days | Review during backlog grooming | Weekly updates if ongoing |
| **P4 – Very Low / Enhancement** | Suggestions, improvements, or nice-to-have features | UI improvements, new report fields, performance tuning | Within 3 business days | Scheduled for upcoming sprint | Handled via normal sprint planning | Updates during sprint planning/demo |

### Additional Notes
- **Response Time:** Time for a developer to acknowledge and start working on the ticket.  
- **Resolution Time:** Time to provide a fix, workaround, or plan.  
- **Escalation Policy:** Immediate escalation if SLA is breached.  
- **Communication:** Regular updates, especially for high-priority tickets.

---

## 📅 Sample SLA Timeline for P1 Ticket

| Time Passed | Action |
|------------|-------|
| 0 min | Ticket created |
| 1 hour | Developer acknowledges ticket, contacts reporter |
| 4 hours | Progress update / initial investigation shared |
| 8 hours | Fix or workaround provided, escalate if unresolved |
| 24 hours | Ticket resolved or detailed plan shared |

---

## 🟨 General Notes

- Emergency fixes (hotfix or rollback) → priority rises to P0, handled ASAP.  
- Bugs needing development: create a bug request, include the bug ID in the support ticket, then close the support ticket.  
- Requests for non-existing actions → redirect requester to business team, then close the ticket.  
- Supporters focus **only on support tasks**.

---

## 🧭 Strategies to Manage High Volume of Support Requests

### 1. 🚫 No Direct Messages or Emails
- Support **must go through official tickets only**.  
- If someone contacts a developer directly, politely ask them to open a ticket.  
- **Exception:** P0 issues may be handled immediately, but a ticket must be opened afterward.  
- ⚠️ **No Git push is allowed without a ticket reference.**

### 2. 👥 Limit Developer Disruption
- Only **assigned weekly supporters** handle support tickets.  
- Other developers focus on tasks.  
- If another developer is required, the supporter involves them **with prior agreement**.

---

## ✅ WFH/WFO Tracking Summary

- **shared Excel sheet** marks **WFO (“O”)**, **WFH (“H”)**, and **Vacation (“V”)**.
- Submit a **timesheet snapshot daily** when working remotely.  
- Regularly **monitor the tracking sheet** to verify your entries and inform me of any missing or incorrect records.

