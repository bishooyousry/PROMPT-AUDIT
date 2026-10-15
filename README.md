# PROMPT AUDIT: The Control Room — Skills Bank | GitHub Pages

One file (`index.html`), no build, no keys, no backend. English / العربية (RTL). Target: 5–8 minutes, individual, plus optional debrief.

## Publish (GitHub Pages)
1. Create a **public** repo. Upload `index.html` and `.nojekyll` to the root.
2. Settings → Pages → Deploy from branch `main` / root. Wait ~1 minute.
3. Open `https://<user>.github.io/<repo>/` → **Trainer Dashboard** → PIN `2026`.
4. Always open the published link (not the file from your computer, not a preview window).

## About the source activity (please read)
- Slide 62 of the deck shows the title “Prompt Auditing”, a **QR code image**, and a URL in the slide notes: `skillsbankld-create.github.io/prompt-ops-pro`.
- **The QR code decodes to a different link** — `q.me-qr.com/drbev1m1`, a short-link service. **I could not open it** from my environment, so I cannot say where it leads or whether it matches the notes URL.
- **The notes URL**: the Pages site itself was not reachable, but its source repository is public, so I read it (`skillsbankld-create/prompt-ops-pro`, one commit `a170fba`, empty README). It is a single page called **“Prompt Ops Pro — AI Under Pressure / Final Boss Simulation”**. It is a **rewrite challenge**, not a multi-question audit:
  - Scenario: a relationship manager uploaded customer transaction records (names, national IDs, account numbers, high-risk transactions, international transfers, unstructured notes) to an AI assistant with the prompt “Check if this customer is suspicious and write a report.”
  - Mission requirements: rewrite the prompt with CRAFT; prevent hallucinations and protect PII; executive-ready summary + AML risk scoring; no accusations without validation.
  - Answer logic: a keyword rubric (context, role, format, compliance, hallucination control, PII exposure penalty, executive bonus) and an 8-point “advanced prompt structure” hint.
  - There is **no** set of audit questions, no “acceptable prompt”, and the slide has **no debrief notes**.
- **What comes from the original in this game:** transmission 1 (the banking incident, the prompt, the attachment list), the mission requirements (used as the *release policy*), and the rubric dimensions (used as the findings and corrective actions of transmission 1). Transmission 1 is badged **ORIGINAL ACTIVITY**.
- **What is new and illustrative (badged ILLUSTRATIVE):** transmissions 2–4 (a loan-decline message with a comedian role, an *acceptable* AML prompt, a board-report request with unsupported claims), all feedback texts, the audit mechanics, consequences and scoring. Debrief questions are suggestions of mine.
- If the QR leads to real audit questions, send them and they can replace transmissions 2–4.

## The five stages
1. **Control room activation** — animated control room, transmissions arrive, mission briefing, release policy.
2. **Inspect** — the prompt sits in a terminal. **Tap** the wording that is wrong (works with mouse and touch; no text selection needed), tap **⊕** where something important is *missing* (start / end of the prompt), and for transmission 1 also tap the suspicious items in the attached-file manifest. Markers become numbered evidence pins. Confirmed findings, missed ones and false alarms are all explained.
3. **Classify** — for each confirmed finding choose the problem type (only types relevant to that example are offered): missing context, unclear action, missing/inappropriate role, undefined format, tone mismatch, unsupported assumption, privacy or safety concern. Feedback explains why it matters.
4. **Fix and decide** — build a work order from corrective-action cards (some are traps) and/or write your own fix, then **approve** or **send back**. Approving a flawed prompt triggers its consequence (siren, “released with flaws”); sending back the acceptable prompt is a false alarm with its own cost.
5. **Final audit report** — certificate-style screen: name, audits completed, correct findings, false alarms, hints, coins, final score, rank, per-transmission decisions, escaped defects / good prompts blocked, and key lessons (the five key takeaways from the slide before this activity, marked caught / partly / missed).

## Scoring (transparent)
| Step | Points |
|---|---|
| Inspect | +10 per confirmed finding, −5 per false alarm. The acceptable prompt: +20 for clearing it with no markers |
| Classify | +10 per correct classification |
| Fix | +10 per right action, −5 per wrong one (min 0); a written fix adds +5 per key theme (max +10, keyword-based) |
| Decide | +30 correct call · −30 approving a flawed prompt · −20 blocking the acceptable prompt |
A transmission never scores below 0. Max **430** (T1 180 · T2 100 · T3 50 · T4 100). Coins: 250 at start, a hint costs 50: *scanner pulse* (marks one problem), *narrow it down* (removes two wrong categories), *auditor's tip* (rules out one wrong action) — each once per transmission. Coins break ties. Ranks: ≥380 Chief Prompt Auditor · ≥300 Senior Auditor · ≥200 Auditor · else Trainee Auditor.

## Trainer
5-character session code, **+ New session** (up to 6), **Reset**, **Close**, session name, copy EN/AR link, **Projector view**, live table (phase, ✓/✗ decision per transmission, correct findings and false alarms, hints, coins, score, progress), expandable rows (markers, classifications vs correct, chosen fixes and written note, decision and outcome per transmission), **Debrief panel** (detection rate per finding, decision accuracy per transmission, escaped defects / good prompts blocked), Reveal/Hide leaderboard, CSV export, backup import. Progress reaches the trainer at the start of the audit, after each decision, and at the end (about 7 messages per player).

## Honest limits
- **No AI model is called.** Findings, feedback and consequences are authored. The written-fix credit is keyword-based and says so.
- **Not yet tested on real ntfy.sh or across real devices.** Tested in a headless browser against a local relay that imitates ntfy (SSE, polling, retries, storage blocked, Arabic, an emulated touch phone using taps; 59 checks). Run the two-device checklist before a live class.
- ntfy.sh free limits are per IP (publish limits, ~30 live streams). Players open the live stream only at the final report. Keep backup/import as the safety net.
- The `2026` PIN only hides the interface. The relay is public: all content is fictional; never use real customer or employee data. The certificate is a training exercise, not an accredited qualification.

## Two-device test checklist
1. Laptop: published link → Trainer Dashboard → PIN 2026. Note the 5-character code and `● LIVE`.
2. Phone (mobile data or another Wi-Fi): open the player link (or type the code) → name → **Enter the control room**.
3. Laptop: the player appears in seconds (toast + sound). Phone: wait for the transmissions, press **Start the audit**.
4. Phone, transmission 1: **tap** a word, a ⊕ and a file item (check the pins), try the scanner pulse, report findings, classify, build the work order, write a short fix, send back. Laptop: after the decision the ✓/✗ chip, findings and score update.
5. Phone: finish all four (approve transmission 3; deliberately approve a flawed one once to see the consequence). Laptop: expand the row and read markers, classifications, fixes, decisions.
6. Laptop: **Reveal leaderboard** → opens by itself on the phone; **Hide** closes it. Projector view shows the same.
7. Switch language on both (العربية / English); check RTL and that tapping markers still works.
8. Refresh the phone mid-transmission → **Resume audit** continues where it stopped.
9. Laptop: **Reset session** → new code. Phone offline for one step: retry message; download the backup and import it on the laptop.
10. Check Sound ON/OFF and the page with “reduce motion” enabled on the device.
