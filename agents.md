Mission File — Email Audit

Analyze exported email data (MBOX) to find open loops and broken commitments — both directions. Work in chunks. Survive resets. Accumulate findings.

⟳ Session Start (Every Time Memory is Compacted)

- Read this file
- Read todos.md — if it doesn't exist, create it first (see Step Zero)
- Read insights.md — if it doesn't exist, create it with sections for:
  - Outbound Open Loops
  - Inbound Open Loops
  - Top 10 Recovery List
- Pick up at the first unchecked item in todos.md
- Process that item, write findings to insights.md, check it off in todos.md
- Repeat until finished

Step Zero: Build the Todo List

Before analyzing anything, scan the MBOX file and create todos.md with:

- Total email count and date range
- Chronological batches of ~20 emails each as checkboxes
- A final section of post-processing tasks as checkboxes

## Email Batches

- [ ] Batch 1: Jan 1 – Feb 15 (~20 emails)
- [ ] Batch 2: Feb 16 – Apr 2 (~20 emails)
- [ ] Batch 3: ...

## Post-Processing

- [ ] Top 10 Recovery List
- [ ] Final review of insights.md

🔍 What to Find

Outbound Open Loops

Sent emails with commitment language ("I'll send," "I'll follow up," "by Friday") where follow-through is missing.

Log:
- date
- recipient
- promise
- follow-through (yes/no/partial)
- still recoverable?
- priority (High/Med/Low)

Inbound Open Loops

Received emails where others made commitments and didn't deliver. Did you follow up?

Log:
- date
- sender
- their commitment
- follow-through
- your follow-up (yes/no)
- recoverable?
- priority

📋 Rules

- One batch per cycle. Check it off before starting the next.
- Always update both files before memory is compacted.
- Never re-process a checked item.
- Be specific: names, dates, short quotes.
- Opportunity framing, not guilt.
- Flag ambiguous items as "low confidence."
- Write at a fifth-grade reading level. Short sentences.
