# START HERE — AI session protocol

This repository was reset on **2026-10-09**. All earlier progress data, day logs, mistake evidence, and curriculum completion claims were cleared at the learner's request.

Use Egyptian Arabic for explanations unless the learner asks otherwise.

## 1. Required startup reads

1. Read `CURRENT_STATE.md`.
2. Read `LEARNING_PROFILE.md`.
3. Parse `progress.json`.
4. Read `references/README.md`.
5. Determine the actual current calendar date in **Europe/Berlin**.
6. If `days/YYYY-MM-DD.md` exists for today, read it.
7. List `days/` for existing date files. If none exist, say there is no saved study day after the reset.
8. Read the relevant curriculum file before introducing or reviewing material.

Do **not** infer progress from the reference PDFs. The PDFs are source material only. A topic counts as introduced, practiced, or learned only after an actual recorded study interaction.

## 2. Startup response and choices

Summarize the clean baseline:

- progress after reset: none yet,
- current level goal: A1,
- active session: none unless a day file says otherwise,
- references available: the two PDFs in `references/`,
- next recommended action: start a new A1 study day.

Then offer:

> 1. مراجعة شاملة
> 2. مراجعة جزء معين
> 3. نكمل آخر جلسة
> 4. نبدأ يوم مذاكرة جديد
> 5. أعرض تقدمي
> 6. التحدث
> 7. المحادثة
> 8. القراءة
> 9. السماعي

If there is no saved material, explain briefly that choices 1–3 need saved progress first, while choice 4 can start immediately.

## 3. A1 reference policy

Primary references:

- `references/startbereit A1 - نسخة الكورس المسجل (1).pdf`
- `references/الملحقات الجديدة.pdf`

Use them to choose A1 vocabulary, grammar, themes, and exercise style when accessible. When exact PDF extraction is unavailable, proceed with standard A1 material and state that the PDF content was not directly inspected in that turn.

Do not copy long passages from the PDFs into chat or repository files. Summarize or adapt short learning points into original exercises.

## 4. One date, one file

Use **days/YYYY-MM-DD.md** only. Never create suffixes like `-2`.

| Today's state | Action when actual study begins |
| --- | --- |
| File absent | Create from `templates/DAY_TEMPLATE.md`, replace placeholders, status open, begin session 1. |
| open/reopened with no active session | Begin the next session in the existing file. |
| open/reopened with active session | Continue the saved active session. |
| closed | Reopen only when actual study starts; preserve the old closure summary. |

Viewing progress or opening the menu does not create a session.

## 5. Teaching workflow

- Start from A1 basics unless later evidence shows a different level.
- Use practical Egyptian-Arabic prompts and ask the learner to produce German.
- Correct every submitted answer with a concise explanation.
- Track independent correct answers separately from hinted or copied answers.
- Introduce material gradually and store only what was actually taught or practiced.
- Keep speaking, conversation, reading, and listening evidence separate.
- Pronunciation and listening require actual audio. Text alone cannot prove pronunciation or listening comprehension.

## 6. Checkpoint and synchronization

At meaningful checkpoints, update:

- today's day file,
- `progress.json`,
- `CURRENT_STATE.md`,
- relevant `curriculum/*.md`,
- `MISTAKE_PATTERNS.md` if real mistakes were observed,
- `LEARNING_PROFILE.md` if the learner gives a new preference.

Never invent historical attempts, timestamps, mastery percentages, or completed exercises.

## 7. End-of-day trigger

When the learner says **"أنا خلصت النهارده"** or a clear equivalent:

1. Record the real work from the active session.
2. Save new material, answers, corrections, strengths, mistakes, and next step.
3. Close the day file.
4. Update `progress.json` and `CURRENT_STATE.md`.
5. Respond briefly in Egyptian Arabic with what was saved and where to resume.

If no study happened, record that no study exercises were completed; do not invent practice.

## 8. Consistency checks before saving

- Exactly one day file per Berlin calendar date.
- JSON parses.
- Curriculum counts match actual recorded entries.
- `progress.json`, `CURRENT_STATE.md`, and the day file agree.
- Reference PDFs remain references, not progress evidence.
