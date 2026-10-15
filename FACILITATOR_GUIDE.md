# Facilitator guide — PROMPT AUDIT: The Control Room (online)

**Goal:** participants act as prompt-quality auditors: spot what is wrong in a prompt, name the type of problem, choose the fix, and make a defensible approve / send-back decision — without blocking prompts that are fine.
**Format:** individual, 5–8 minutes of play + 5–7 minutes of optional debrief.

## Know the source before you present
- The slide’s QR code opens a short link I could not verify; the URL in the slide notes opens “Prompt Ops Pro — AI Under Pressure”, a *rewrite* challenge about one banking incident. Transmission 1 of this game is that incident; transmissions 2–4 are illustrative examples (badged on screen). The slide has no debrief notes, so the questions below are suggestions.
- Heads-up about the original web activity (if you also use it): its keyword scoring subtracts 15 points whenever the prompt text contains “account number”, “national id” or “customer name” — even in a protective sentence such as “names and national IDs have been replaced with codes”. A good, anonymized prompt can therefore be penalized there. In this game the acceptable prompt (transmission 3) deliberately uses those words protectively.

## Before the session (5 min)
- Open the link → Trainer Dashboard (PIN 2026). One session per group (**+ New session**).
- Put the **player link** (or the 5-character code) in the chat. An Arabic link is available.
- Tell participants: sound is optional (🔊), tapping works on phones, everything is fictional, and **never paste confidential data into any AI tool**.

## Run (timing)
| Time | What you do |
|---|---|
| 0:00 | Say: “You are now the quality auditor. Four prompts are waiting for release — some are fine, some are not. Your decisions have consequences.” Share link/code. |
| 0:01 | Everyone is in. Optionally open **Projector view**. |
| 0:01–0:08 | Watch the table: ✓/✗ decision chips, findings, false alarms, hints, score. Expand a row (⌄) to see exactly what a player marked, how they classified it and what they decided. |
| ~0:08 | When most are done: **Reveal leaderboard** (players see it automatically) or use Projector view. |
| 0:08–0:15 | Debrief (below). |

## What happens in the game (for narration)
1. **Inspect** — tap the wrong wording; tap ⊕ where something is missing. Over-flagging costs points: not every part of a prompt is a problem.
2. **Classify** — why is it a problem? (context, action, role, format, tone, assumption, privacy). Only relevant types are offered.
3. **Fix** — choose corrective actions (some sound good but are traps) or write your own.
4. **Decide** — approve or send back. Approving a flawed prompt has a consequence; blocking a good one is also a failure.
5. **Report** — certificate-style summary with the key lessons from the slide before this activity.

## Debrief questions (suggested)
1. **Which issue did most people miss?** (Detection bars on the dashboard: the lowest bar.) Why is a *missing* thing harder to see than a wrong thing?
2. **Did anyone approve the risky prompt?** What made it look acceptable? (Escaped defects counter.)
3. **Transmission 3 was fine.** Did anyone block it or flag parts of it? Why is blocking a good prompt a cost too? What would you check before approving a prompt in your own team?
4. **Transmission 1:** which safeguards would you add first — role, anonymization, output format, guardrails? Which data must never reach an AI tool without anonymizing?
5. **“Suspicious”** asks the AI for a verdict on a person. How would you rephrase it so a human stays in charge of the decision?
6. Who in your organization should own prompt review before a prompt is released (prompt library, approvals, compliance)?

## Notes
- Automatic scoring is rule-based and transparent; the written-fix credit is keyword-based. Use the results for feedback, not for grading people.
- Progress reaches the dashboard at the start, after each decision and at the end — a player may look idle between decisions.
- If the live connection drops: **Refresh** on the dashboard rebuilds from the relay history; otherwise collect backup files and use **Import**.
- Export CSV at the end if you want to keep the results.
