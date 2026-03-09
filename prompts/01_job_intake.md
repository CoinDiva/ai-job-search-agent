# Prompt 01 — Job Intake (Input Normalizer)

**Goal:** Convert any job post into a clean, structured intake that the agent can score and generate assets from.

## Instructions for the user
Paste the full job description below. If available, include:
- Company name + role title
- Location + remote/hybrid details
- Salary range (if listed)
- Link to job post (preferred: official careers page)

Then answer the questions at the end.

---

## Prompt (copy/paste into ChatGPT)

You are an AI Job Search Agent. Your first task is to normalize the job description into a structured summary.

### Output format (use headings + bullet points)

**1) Role Snapshot**
- Company:
- Title:
- Location:
- Remote/Hybrid:
- Salary range:
- Employment type (FT/PT/Contract):
- Reports to (if stated):
- Team / function:

**2) What This Role Owns (Responsibilities)**
- Top 8–12 responsibilities (bulleted)

**3) Must-Have Requirements**
- Top 8–12 required skills/experiences (bulleted)
- Tools/platforms mentioned (bulleted)

**4) Nice-to-Have Requirements**
- Top 5–10 preferred skills/experiences (bulleted)

**5) Keywords & Signals**
- 15–25 ATS keywords (comma-separated)
- Any “red flag” requirements (e.g., heavy coding, ML model building, SQL/Python as core, technical PM roadmap ownership)

**6) My Quick Fit Questions (for the candidate)**
Ask me up to 6 questions to fill gaps you need before scoring (keep them simple).

---

## Job Description (paste below)
[PASTE JOB DESCRIPTION HERE]

---

## Candidate Notes (answer briefly)
1) What role types are you targeting (pick 2–3)?
2) What industries do you prefer (if any)?
3) Must be remote? (Y/N)
4) Compensation minimum (if you have one):
5) Any deal-breakers (travel %, tech stack, etc.)?
