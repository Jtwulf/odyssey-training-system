# PLAN Operations Rules

Last updated: 2026-08-23

This file is the canonical operating rulebook for how Odyssey Training System writes, maintains, and visually presents the Google Sheets `PLAN`.

It complements:

- `knowledge/evidence.md` — the lightweight evidence index and topic-routing entry point;
- `knowledge/evidence/` — detailed scientific claims and verified references;
- `knowledge/coaching-system.md` — how evidence is translated into Odyssey coaching logic;
- Google Sheets `PLAN` — the actual WHAT / WHEN.

The monthly workout plan itself must **not** be copied into GitHub.

---

## 1. Persistence and rule ownership

### Canonical rule storage

- **GitHub is the Source of Truth for persistent WHY / HOW / operating rules.**
- Google Sheets `SYSTEM` may contain a short convenience summary of operating rules, but it is **not** the canonical rule store.
- Chat history, project memory, assistant memory, or an earlier conversation may help recover context, but they must **not** be treated as the durable Source of Truth for a rule that is intended to govern future plan creation.

### When a conversation change becomes a persistent rule

If the user gives a correction or preference that is clearly intended to apply to future Odyssey planning — for example:

- how time-based vs distance-based work should be chosen;
- how Workout Details should be formatted;
- how milestone rows should appear;
- which fields belong in PLAN;
- how recovery should be described;
- how future dates should be pre-created;
- how announced workouts may or may not be changed;

then that adjustment should be written into this GitHub rulebook in the same workflow, rather than being left only in chat context.

### Conflict handling

- The latest explicit user instruction overrides an older operating rule.
- When that happens, update the relevant GitHub rule so the repository and future behavior agree.
- Do not silently rely on a remembered correction that contradicts the repository.

---

## 2. Required workflow before editing PLAN

For a meaningful monthly-plan creation or revision:

1. Read the current relevant rules in `coaching-system.md` and this file.
2. Read `evidence.md`, identify the milestone/workout-family routing, and load only the relevant detailed topic files from `knowledge/evidence/`.
3. Read the current Google Sheets `PLAN` before writing.
4. Preserve already-announced Main Workout structures unless a justified change is explicitly being made.
5. Apply the requested revision.
6. Re-read the affected PLAN range after writing and verify dates, workout structure, milestone placement, formatting-sensitive text, and row readability.
7. For evidence-sensitive revisions, verify that the participant-facing `Training Effect` remains inside the cited Claim boundaries.

Do not load every evidence file by default. Read `references.md` when verifying, challenging, or updating a scientific claim—not for routine PLAN display work.

---

## 3. Time-based vs distance-based work

### No default unit

There is **no rule that time-based work is the default and distance-based work is the exception**, or vice versa.

For every interval session, actively choose the unit that best serves the primary training purpose.

### Prefer time-based work when

- comparable **work duration at the target intensity** across a heterogeneous group is central to the session;
- a fixed distance would create materially different work-bout durations between groups and that difference would distort the intended stimulus;
- the main target is a physiological domain such as controlled threshold duration or aerobic-power exposure rather than learning a specific race distance;
- group execution is clearer with common start/stop times.

Examples: `3 × 6 min threshold`, `5 × 3 min aerobic power`.

### Prefer distance-based work when

- race-distance specificity or learning the feel of a defined distance matters;
- the goal includes pace judgment over 200 m / 300 m / 400 m / 600 m / 800 m / 1 km or another meaningful segment;
- the venue provides reliable fixed landmarks that improve execution;
- exact distance improves participant understanding or race-rhythm rehearsal;
- different work durations across groups are acceptable for the session objective.

Examples near a 1 km event: controlled `600 m` speed-endurance repetitions or low-volume `300 m` sharpening repetitions.

### Important implementation rules

- **Do not choose time-based work solely because the group has mixed ability.** Mixed ability is one consideration, not the answer by itself.
- **Do not force a 50/50 mix of time and distance.** Variety must come from training purpose, not aesthetics.
- Work unit and recovery unit are independent. A distance-based repetition may use a time-based recovery, and vice versa.
- Distance equality does not imply stimulus equality. Consider expected rep duration for each group before approving a distance-based session.
- Before finalizing a monthly plan, explicitly ask: `Why is this workout time-based or distance-based?` If there is no objective answer, reconsider the prescription.

---

## 4. PLAN row content

The standard PLAN columns are:

`Date | Focus | Venue | Main Workout | Workout Details | Training Effect | Group A | Group B | Group C | Group D | Notes`

`Recovery`, `Warm-up`, and `Cooldown` are intentionally **not separate columns**. Their complete operational detail belongs in `Workout Details`, while the main-set recovery is also summarized in `Main Workout` when relevant. Do not duplicate the same instructions across separate columns.

### Main Workout

Keep it scannable. Normally use no more than two short lines:

```text
<main set>
<recovery>
```

Recovery wording must make clear whether it is:

- easy jog;
- walk / jog;
- standing / passive;
- none / continuous.

### Workout Details

Markdown rendering is not assumed. Use plain text, line breaks, and blank lines.

Always use this order:

```text
【WU】
...

【PREP】
...

【MAIN】
...

【RECOVERY】
...

【CD】
...
```

Include enough detail that the session can be run from the cell without reconstructing missing instructions:

- WU distance or duration;
- drills / preparation where used;
- strides / accelerations including number and approximate distance;
- exact main set;
- recovery duration or distance;
- whether recovery is jog, walk-jog, standing, or none;
- CD distance or duration.

Do not add drills merely to make the session look sophisticated. Preparation must match the session need.

### Training Effect

- 2–3 short Japanese lines.
- State what the workout is intended to stimulate and how that can help running.
- Keep it understandable without physiology jargon.
- Do not claim the exact prescription guarantees an adaptation or race result.
- It should remain substantially true if one group's pace or repetition count is modestly adjusted on the day.

### Notes

Use `Notes` for operational context such as race proximity, weather/heat adjustment, execution cautions, recalibration conditions, and group-specific exceptions. Do not use it to duplicate WU / PREP / MAIN / RECOVERY / CD instructions already present in `Workout Details`.

---

## 5. PLAN visual hierarchy

### General layout

- Header row remains frozen.
- Cells use wrap and top alignment for normal workout rows.
- `Workout Details` is the widest content column.
- Use line breaks and blank lines instead of Markdown syntax.
- The first Tuesday row of a new calendar month receives a stronger top border to show the month boundary.

### Workout-row height / clipping prevention

- A populated workout row must be tall enough that the full wrapped `Workout Details` text is visible without clipping.
- Do **not** assume Google Sheets auto-resize will correctly size heavily line-broken cells. If auto-resize produces a row that is too short, set an explicit row height.
- After writing or materially changing `Workout Details`, verify the affected row height as part of the post-write read/check workflow.
- With the current `【WU】 / 【PREP】 / 【MAIN】 / 【RECOVERY】 / 【CD】` format, roughly **260–285 px** is a practical baseline for populated rows, but this is an operational starting point rather than a mandatory fixed height. Use less or more when the actual content requires it.
- Milestone rows and future `Date`-only rows should remain compact; do not expand them to workout-row height.
- Readability takes priority over keeping all workout rows visually identical in height.

### Milestone rows

For an important race or event that should be visible in the training sequence:

- insert a dedicated row chronologically between the surrounding Tuesday sessions;
- merge the full PLAN width for that row;
- use a light-yellow background;
- use bold text;
- **left-align** the text;
- show **only** `date ｜ race/event name`;
- do not prepend labels such as `MILESTONE`.

Example:

```text
2026-09-19 ｜ DESCENTE 1 km TIME TRIAL
```

### Future Tuesday rows

- Future Tuesdays may be pre-created with the `Date` field only.
- Leave the other fields blank until that period is actually designed.
- Pre-creating dates does not mean the workout has been approved.

---

## 6. Plan revision rules

### Before public announcement

The PLAN may be structurally redesigned when the evidence, milestone logic, venue, or user feedback supports a better solution.

### After public announcement

Preserve the announced Main Workout structure unless there is a meaningful safety, logistical, or explicitly approved coaching reason to change it.

Normally adjustable without changing the identity of the session:

- pace ranges;
- group count and assignments;
- heat/environment adjustment;
- modest recovery adjustment;
- shortening for one group;
- explanatory wording and operational detail.

A change such as `1 km × 5` to an unrelated `400 m × 12` is a structural change and should not happen casually after announcement.

---

## 7. Evidence audit of a future PLAN row

Before considering a session ready, verify:

1. The primary `Focus` maps to at least one relevant Evidence Claim.
2. The `Training Effect` describes the supported target/transfer rather than promising a result.
3. Acute response, chronic adaptation, and race-performance evidence have not been conflated.
4. Evidence strength and directness to Odyssey are understood separately.
5. Exact pace, repetition count, and recovery are marked mentally as coaching prescriptions rather than uniquely proven constants.
6. Expected rep duration and total quality dose are reasonable for every proposed group.
7. Environment and 60-minute logistics do not materially distort the intended stimulus.
8. If current-performance information is incomplete, the first repetition or an earlier related session is used for conservative recalibration.

An evidence audit does not require Claim IDs to be displayed in the Google Sheet. Keep PLAN participant-facing and operationally readable.

---

## 8. Rule-maintenance check

At the end of a planning conversation, ask internally:

1. Did the user make a correction that should affect future plans?
2. Is that correction already represented in GitHub?
3. If not, should `coaching-system.md`, `plan-operations.md`, `evidence.md`, a routed topic file, or `references.md` be updated?
4. Is the Google Sheet only storing WHAT / WHEN and a convenience SYSTEM summary, rather than becoming the sole home of a durable HOW rule?
5. Did a new or corrected scientific claim trigger an audit of affected future PLAN rows?

If a future-facing rule exists only in chat, persistence is incomplete.
