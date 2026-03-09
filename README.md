# ai-job-search-agent
# AI Job Search Agent (ChatGPT)
Project URL: https://github.com/CoinDiva/ai-job-search-agent
A prompt-driven “AI agent” that helps identify high-fit remote AI roles and generates application-ready outputs: fit score, Apply/Strong Apply/Stretch/Skip recommendation, ATS keywords, tailored resume bullets, LinkedIn outreach, cover letter opening, and interview prep questions.

> Built as a Project Management + GenAI workflow project. Tool-agnostic: works in ChatGPT, Claude, or Gemini.

---

## Project Goal

Create a repeatable, professional job search workflow for remote AI roles (business-side) that reduces search time and improves application quality and consistency.

**Target roles**
- AI Partnerships Manager
- AI Solutions Consultant
- AI Go-To-Market Strategy Lead
- AI Product Marketing Manager
- AI Customer Success Director
- AI Adoption Specialist
- AI Program Manager / Project Manager (non-technical, operations/adoption-focused)
- Strategic Partnerships Manager
- Brand Partnerships Manager (AI companies)

**Priority constraints**
- Remote-first
- Business-side AI roles (not engineering)
- Penalize roles requiring heavy coding, ML model building, or technical PM roadmap ownership

---

## What This Agent Produces (Outputs)

For any job description, the agent returns:

1. Company, title, location, salary (if listed), key required skills  
2. Score (0–100) using a weighted rubric  
3. Recommendation: Apply / Strong Apply / Stretch Apply / Skip  
4. ATS keywords list  
5. Tailored resume bullet rewrites (truthful + metrics-driven)  
6. LinkedIn outreach message (recruiter + hiring manager versions)  
7. Cover letter opening paragraph  
8. Interview questions + prep angles  
9. Best next step: Apply Now / Network First / Tailor Resume First  

---

## Repo Contents

- `/prompts` — copy/paste prompt templates for each step
- `/examples` — sample job descriptions + generated outputs
- `/templates` — tracker templates (CSV) and project overview text

---

## How To Use (Fast)

### Step 1 — Copy the prompts
Open the `/prompts` folder and run prompts in order:

1) `01_job_intake.md`  
2) `02_scoring_rubric.md`  
3) `03_tailored_resume_bullets.md`  
4) `04_linkedin_outreach.md`  
5) `05_cover_letter_opening.md`  
6) `06_interview_questions.md`  
7) `07_daily_scan_workflow.md` (optional)

### Step 2 — Paste a job description
Paste the full job description into the agent along with your resume highlights (or a link to your resume).

### Step 3 — Save outputs
Paste final outputs into your tracker (see `/templates/scoring_sheet_template.csv`) and save the role outcome.

---

## Scoring Rubric (Summary)

**Weighted rubric (100 points)**
- Role alignment: 25
- Transferable experience: 20
- AI readiness match: 15
- Seniority match: 10
- Industry match: 10
- Remote / compensation practicality: 10
- ATS keyword alignment: 10

**Automatic penalty (10–20 points) if central requirements include:**
- software engineering
- ML model development
- technical product management with roadmap ownership
- SQL/Python/analytics stack as core requirements
- AI startup experience listed as mandatory

**Recommendation bands**
- 85–100 = APPLY NOW
- 70–84 = STRONG APPLY
- 55–69 = STRETCH APPLY
- <55 = SKIP

---

## Guardrails (Important)

- Human review before sending anything externally
- No sensitive personal info in prompts
- Keep claims factual; don’t invent experience
- Prefer company career pages over job boards
- Flag “attractive titles” that are actually technical/engineering roles

---

## Success Metrics

- Time saved per application (minutes)
- # of “Strong Apply” roles identified per week
- Response rate from recruiter outreach
- Interview conversion rate

---

## License

No license currently. Add one if you want others to reuse the framework.

---

## Built By

Beth Silverberg — AI Adoption + GTM Partnerships  
LinkedIn: https://www.linkedin.com/in/bethrobyn/
