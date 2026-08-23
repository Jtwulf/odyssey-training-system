# Odyssey Coaching System

Last updated: 2026-08-23

This file translates `evidence.md` into operating rules for Odyssey Running's Tuesday Quality Session.

Every meaningful rule should be read with one of three labels:

- **[Evidence-based]** — directly supported by reasonably applicable research.
- **[Inference]** — a reasonable translation of research into Odyssey's constraints, but not directly tested in this exact setting.
- **[Coaching judgment]** — an operational choice required to run the session; it must not be presented as something uniquely proven by research.

---

## 1. System boundary and Source of Truth

### Scope

- **[Coaching judgment]** Odyssey manages the Tuesday **20:00–21:00 Quality Session / Point Workout**.
- **[Coaching judgment]** Typical attendance is **5–10 runners** with a wide ability range.
- **[Coaching judgment]** Planning is presented in **calendar-month units**, while the underlying training logic remains milestone- and progression-aware.
- **[Coaching judgment]** Primary venues through the current cycle are **Yoyogi Park** and **Meiji Jingu Gaien**.

### Non-scope

- **[Coaching judgment]** Do not manage each participant's weekly mileage, sleep, fatigue, injury history, Strava history, or individual weekly plan.
- **[Coaching judgment]** Do not import Justin's personal JTBC training state, injury history, or personal race targets into Odyssey decisions.
- **[Inference]** Whole-program concepts such as polarized/pyramidal TID are background constraints, not Tuesday-only targets, because Odyssey controls only one session per week.

### Source of Truth

```text
GitHub
= WHY / HOW
= Evidence + Coaching Logic

Google Sheets
= WHAT / WHEN
= actual monthly Workout Plan

Strava
= public participant announcement
```

- **[Coaching judgment]** Never duplicate the monthly Workout Plan into GitHub.
- **[Coaching judgment]** Do not add Draft / Review / Approved / Locked workflow states unless a future operational problem clearly requires them.

---

## 2. Core design principles

1. **[Evidence-based]** Quality training should not be reduced to one repeated intensity. Threshold, aerobic-power/VO2, speed-oriented, hill and race-specific stimuli can all have roles across a training cycle.
2. **[Inference]** The goal is not for every runner to cover the same distance. The goal is for runners to receive a **comparable training stimulus appropriate to the session objective**.
3. **[Evidence-based]** Interval prescription has multiple interacting variables and the literature does not establish one universally optimal combination of work duration, intensity and recovery.
4. **[Coaching judgment]** Therefore exact rep counts, recovery lengths and pace bands are chosen to satisfy the current objective, milestone, venue and 60-minute operating window.
5. **[Evidence-based]** Specificity should increase as an important event approaches, while total load is reduced near competition rather than simply making every week harder.
6. **[Coaching judgment]** Progression does **not** mean “harder every Tuesday.” It can mean more specificity, better pace control, a different stimulus, reduced recovery, increased quality volume, or deliberate unloading/sharpening.
7. **[Coaching judgment]** Easy/social running is not the main Tuesday workout. Easy running remains part of warm-up, recovery and cooldown.

---

## 3. Monthly planning method

For each calendar month, design all Tuesdays together before announcement.

### Step A — identify milestones

- **[Coaching judgment]** List races/events that materially affect multiple members.
- Current milestones:
  - **2026-09-19 — DESCENTE 1 km Time Trial**
  - **2026-11-01 — Seoul Marathon**

### Step B — define the month-level training problem

- **[Inference]** Decide which qualities need emphasis based on the next milestone while maintaining enough variation that the month is useful to non-participants too.
- Examples of qualities: threshold durability, aerobic power, speed endurance, short-speed/neuromuscular quality, hills, race-specific rhythm.

### Step C — assign a purpose to each Tuesday

- **[Coaching judgment]** Every session must have one primary `Focus` that can be explained in one short phrase.
- **[Coaching judgment]** Do not choose a workout first and invent the purpose afterward.

### Step D — check progression and fatigue

- **[Evidence-based]** Training emphasis should progress toward event-specific work as competition approaches; pre-race taper evidence favors reducing load while retaining some intensity.
- **[Inference]** A session only four days before an important 1 km TT should generally emphasize sharpening/readiness and avoid large residual fatigue rather than trying to create a new fitness adaptation at the last moment.
- **[Coaching judgment]** The exact low-volume sharpening session remains a coaching prescription, not a directly proven four-day formula.

### Step E — check the 60-minute constraint

- **[Coaching judgment]** The full session—warm-up, preparation, main work, recovery and cooldown—must fit inside 20:00–21:00 with realistic transitions.
- **[Coaching judgment]** If a mathematically elegant workout does not fit operationally, it is not an Odyssey workout.

---

## 4. Standard 60-minute session architecture

### Default architecture

```text
20:00–20:10/12  Easy running
20:10/12–20:16/18  Dynamic preparation
20:16/18–20:20  Optional progressive strides / workout-specific prep
~20:20–20:48/50  Main workout
~20:48/50–20:58  Easy cooldown
20:58–21:00  Finish / regroup
```

### Why this structure exists

- **[Evidence-based]** Warm-up generally improves subsequent physical performance.
- **[Evidence-based]** Prolonged static stretching immediately before speed/explosive work has no demonstrated advantage and can impair explosive performance in some contexts.
- **[Inference]** Easy running followed by dynamic preparation and, on faster days, progressive strides provides a practical progression from low intensity toward workout speed.
- **[Coaching judgment]** The exact minute split above is chosen to fit Odyssey's 60-minute window; research does not prove that 10–12 minutes plus 6 minutes of drills is uniquely optimal.

### Warm-up by workout type

#### Threshold / controlled tempo day

- **[Coaching judgment]** 10–12 min easy running.
- **[Coaching judgment]** Short dynamic preparation focused on range of motion and readiness.
- **[Coaching judgment]** 0–3 progressive strides depending on weather, venue and starting pace.
- **[Inference]** Avoid spending excessive time on maximal-speed preparation when the main session does not require it.

#### VO2 / 1 km / speed-endurance day

- **[Coaching judgment]** 10–12 min easy running.
- **[Coaching judgment]** Dynamic preparation.
- **[Inference]** Add 2–4 progressive strides or short controlled accelerations so the first hard repetition is not the first exposure to faster running.

#### Hill / short-speed day

- **[Coaching judgment]** 10–12 min easy running plus dynamic preparation.
- **[Inference]** Include progressive accelerations before maximal or near-maximal hill/speed work because of the higher neuromuscular demand.

### Cooldown

- **[Coaching judgment]** Default 7–10 min easy running where logistics allow.
- **[Coaching judgment]** Cooldown is not allowed to make the main set exceed the one-hour session window; preserve the agreed finish time.

---

## 5. Workout families and when to use them

### Threshold / tempo / cruise intervals

- **[Evidence-based]** Threshold-zone work is a common and useful component of distance-running training, but threshold-dominant total training is not established as superior.
- **[Inference]** Use continuous tempo when a stable sustained rhythm is the main goal and the venue can support uninterrupted running.
- **[Inference]** Use cruise intervals when brief recovery improves pace control, group management or quality volume without changing the session into a VO2 workout.
- **[Coaching judgment]** Formats such as 20 min continuous, 3 × 8 min, or 2 km repetitions are options—not scientific constants.

### Aerobic power / VO2 intervals

- **[Evidence-based]** Work intervals of roughly ≥2 min are effective for accumulating time at high oxygen uptake; longer intervals often accumulate more time near VO2max than very short repetitions.
- **[Inference]** For a mixed group, 3–5 min work bouts are often a useful design space because they can create a meaningful aerobic-power stimulus without requiring identical distances.
- **[Coaching judgment]** Do not prescribe a fixed pace from marathon target alone. Use recent relevant performance and the target physiological/competitive demand.

### 1 km / middle-distance-specific work

- **[Evidence-based]** 800–1500 m performance depends on both substantial aerobic and anaerobic contributions.
- **[Inference]** A 1 km TT therefore benefits from a combination of aerobic power, speed, speed endurance and race-specific rhythm rather than repeated all-out 1 km efforts every week.
- **[Coaching judgment]** Use exact 1 km repetitions only when they solve a specific training or venue problem; they are not automatically the best way to train for a 1 km race.

### Short speed / neuromuscular stimulus

- **[Evidence-based]** Sprint-oriented training can improve speed and anaerobic qualities; strength/plyometric work can improve running economy over multi-week programs.
- **[Inference]** Small doses of high-quality fast running can complement aerobic training, especially before a short race, but should be kept distinct from exhausting sprint-interval work.
- **[Coaching judgment]** Short fast reps should stop before mechanics visibly deteriorate when the session purpose is speed quality rather than fatigue tolerance.

### Speed endurance

- **[Evidence-based]** Sprint/HIIT literature supports training both aerobic and anaerobic performance qualities, but the exact best dose for distance runners is uncertain.
- **[Inference]** Use speed-endurance sessions when the goal is to sustain speed above longer-distance race rhythm under controlled accumulating fatigue.
- **[Coaching judgment]** Do not equate “speed endurance” with maximal sprinting or make it a weekly default.

### Hills

- **[Evidence-based]** Uphill intervals can create meaningful aerobic and neuromuscular overload; no single hill protocol is proven optimal.
- **[Coaching judgment]** Hills are an occasional tool, not a mandatory recurring weekly category.
- **[Coaching judgment]** Yoyogi's ~100 m hill can be used for short hill work when the monthly objective calls for it.

### Marathon-oriented controlled intervals

- **[Evidence-based]** World-class and recreational marathon evidence supports the importance of large low-intensity volume and increasing race-specific work closer to competition, but Odyssey cannot manage those total-program variables.
- **[Inference]** After the 1 km milestone, Tuesday sessions can gradually include longer controlled intervals / sustained work with greater marathon relevance while remaining useful to non-marathoners.
- **[Coaching judgment]** Do not turn every Tuesday into marathon-pace running simply because Seoul Marathon is approaching.

---

## 6. Pace-group system

### Group identity

- **[Coaching judgment]** Group A / B / C / D are **Workout Target Groups**, not permanent runner rankings.
- **[Coaching judgment]** A runner can be A on threshold day and B on short-interval day.
- **[Coaching judgment]** Sex is not used to assign groups; current performance for the relevant workout is.
- **[Coaching judgment]** Use 2, 3 or 4 groups depending on attendance and ability distribution. Do not create empty complexity merely to preserve a fixed number of groups.

### Pace-setting hierarchy

Use the most relevant information available in this order:

1. **[Inference]** recent performance in the same or similar workout/race distance;
2. **[Inference]** recent race performance close to the session demand;
3. **[Inference]** stable threshold/aerobic-power training history;
4. **[Coaching judgment]** broader race targets (including marathon target) only when more specific information is unavailable;
5. **[Coaching judgment]** conservative first-rep calibration when uncertainty remains.

### Pace display

- **[Coaching judgment]** PLAN should normally show **pace ranges**, e.g. `3:40–3:45/km`, not false precision such as a single second per kilometer.
- **[Coaching judgment]** For time-based short work, speed may instead be expressed by a practical split/range or effort cue if pace-per-km becomes misleading.

### Initial field calibration — not a permanent pace table

These are observed Odyssey settings and must only be used as starting context:

- 2 km repetitions, 2 min rest: fastest ~3:40–3:50/km; next ~4:10/km; slower ~5:00/km.
- 1 km repetitions: fastest ~3:30/km; next ~3:40–3:50/km; next ~4:20–4:30/km.

- **[Coaching judgment]** Recalibrate from actual attendance and recent workout performance rather than preserving these values indefinitely.

---

## 7. Distance-based vs time-based intervals

### Primary rule

- **[Inference]** When the objective depends mainly on spending a comparable duration at a target intensity, prefer **time-based work bouts** if fixed distances would create very different work durations between groups.
- **[Coaching judgment]** Example design space: `N × 4 min`, with group-specific speeds and a common time-based recovery.

### When distance-based work is preferred

- **[Inference]** Use distance-based repetitions when race specificity is important, when fixed landmarks simplify execution, or when the venue naturally supports a clean rep structure.
- **[Coaching judgment]** Distance-based work is acceptable even when groups finish at different times if the resulting physiological difference is intended or operationally acceptable.

### Important caveat

- **[Evidence-based]** Interval duration changes the physiological response; research does not support treating a 3:30 rep and a 5:00 rep as identical merely because both are “1 km.”
- **[Inference]** Therefore distance equality is not stimulus equality in a heterogeneous group.

---

## 8. Recovery design

### General rule

- **[Evidence-based]** Active recovery is not universally superior to passive recovery. Both can support interval-training adaptations, and acute runner data show similar time near VO2max under some active/passive comparisons.
- **[Coaching judgment]** Choose recovery mode and duration according to what the next repetition is supposed to look like.

### Practical logic

- **[Inference]** For aerobic-power intervals, recovery should be long enough to preserve the intended work quality but not so long that the session repeatedly returns to a fully reset state when cumulative aerobic strain is the goal.
- **[Inference]** For short-speed work, longer/passive recovery can be appropriate when maintaining mechanics and speed is more important than metabolic density.
- **[Inference]** For threshold/cruise work, short easy-jog recovery can preserve continuity while permitting pace control.
- **[Coaching judgment]** Exact recovery values remain session-specific and must fit the 60-minute window.

---

## 9. Venue logic

### Yoyogi Park

Available characteristics:

- ~1 km usable section
- ~2 km loop
- ~100 m hill usable for hill repetitions

Rules:

- **[Coaching judgment]** Do not maintain a detailed GPS-course database unless an actual operational need appears.
- **[Coaching judgment]** Select the section/loop based on the workout being designed.

### Meiji Jingu Gaien

Representative loop:

- **~1.325 km**

Known operational format:

```text
1 km hard
+ remaining ~300–325 m jog
= one loop
```

- **[Coaching judgment]** This format is operationally simple and can be used when that advantage matters.
- **[Evidence-based]** Work duration and recovery duration influence interval stimulus.
- **[Inference]** Because faster and slower groups take different times for both the 1 km work and ~325 m jog, this loop format does not produce identical physiological dosing across groups.
- **[Coaching judgment]** If comparable recovery duration is important, use a time-based recovery or alter start/re-group logistics rather than assuming the remaining loop automatically solves recovery prescription.

---

## 10. Announcement stability

Once a calendar month's plan has been announced publicly:

- **[Coaching judgment]** Preserve the **Main Workout structure** unless there is a real safety/logistical reason to change it.
- **[Coaching judgment]** Allowed day-of adjustments include:
  - pace ranges;
  - number of groups;
  - group assignment;
  - heat/environment adjustment;
  - modest recovery adjustment;
  - shortening reps for an individual group.
- **[Coaching judgment]** Avoid changing a published `1 km × 5` into an unrelated `400 m × 12` simply because another workout seems more attractive that week.

This is an operational commitment rule, not a scientific claim.

---

## 11. Current milestone logic

### 2026-09-19 DESCENTE 1 km Time Trial

- **[Evidence-based]** 800–1500 m performance is mixed aerobic/anaerobic; aerobic-power interval evidence favors meaningful multi-minute work for accumulating high oxygen uptake; sprint-oriented work can train speed/anaerobic qualities.
- **[Inference]** The 9/1, 9/8 and 9/15 progression should therefore develop complementary qualities rather than repeat all-out 1 km trials.
- **[Evidence-based]** Taper evidence supports reducing load while retaining some intensity before competition.
- **[Inference]** 9/15, four days before the TT, should avoid large residual fatigue and function as sharpening/readiness rather than a maximal training-load day.
- **[Coaching judgment]** Exact workout choices belong only in the Google Sheet PLAN after the evidence base is consulted.

### 2026-11-01 Seoul Marathon

- **[Evidence-based]** Marathon training practice/evidence supports more race-specific work as the main event approaches while maintaining varied training within a largely low-intensity whole program.
- **[Inference]** After the 1 km TT, Odyssey can shift some Tuesday emphasis toward longer controlled work, threshold durability and marathon-relevant rhythm.
- **[Coaching judgment]** Sessions must remain broadly valuable to runners not racing Seoul, and Odyssey does not attempt to provide their complete marathon plan.

---

## 12. Historical Odyssey sessions — field calibration only

These sessions are recorded as operational history, **not** as evidence that the formats were optimal.

### 2026-06-09 — Intervals.icu `i155686940`

- Odyssey session.
- Oda Field.
- `800 m × 6`.
- Fast side approximately 3:10/km by user report.
- **[Coaching judgment]** User report takes priority over unreliable automatic split interpretation for the workout structure.

### 2026-07-14 — Intervals.icu `i165991824`

- Odyssey session, Yoyogi.
- `20 min pace run / tempo`.
- Approx. fast 3:50/km; B ~4:30/km.
- Participants could self-adjust if unable to sustain the planned pace.
- Operational feedback: good fit for Yoyogi.

### 2026-07-21 — Intervals.icu `i167711146`

- Odyssey session, Gaien.
- `1 km × 4`.
- Fast side approximately 3:40/km.
- Recovery = remaining ~300–325 m of the 1.325 km loop as jog.
- Operational feedback: easy to run as a group session.

### 2026-08-04 — Intervals.icu `i172341372`

- Odyssey session, Yoyogi.
- ~100 m hill dash × 15.
- Operational feedback: useful occasionally, not as a frequent default.

### Explicit exclusions

- 2026-08-11 — not Odyssey.
- 2026-08-18 `i177181493` — not Odyssey.
- 2026-07-07 — not confirmed; do not register as Odyssey history without new evidence.

---

## 13. What the system must never claim

Do **not** write statements such as:

- “1 km × 4 with 2 min recovery is scientifically optimal.”
- “Group A must always run 3:40/km.”
- “Active recovery is always better.”
- “Polarized training proves Tuesday should be VO2 every week.”
- “Everyone should run the same distance to receive the same workout.”
- “Four Tuesdays form a scientifically mandatory block.”

Instead use the pattern:

```text
Evidence says: <broad supported principle>
Inference says: <how that principle maps to this month / group / venue>
Coaching judgment says: <the exact operational prescription>
```

---

## 14. Design quality check before a monthly PLAN is written

For each proposed Tuesday, verify:

1. What is the **primary training purpose**?
2. Which evidence principle supports that purpose?
3. Is the exact prescription clearly separated from what the evidence directly proves?
4. Does work duration create a reasonably comparable stimulus across ability groups?
5. Are groups based on this workout, not permanent runner rank?
6. Is recovery chosen for a purpose rather than copied from habit?
7. Does the venue help or distort the intended stimulus?
8. Does the entire session fit 20:00–21:00 including warm-up and cooldown?
9. Does the session make sense in the sequence of the calendar month and next milestone?
10. If close to a race, is fatigue cost justified?
11. Is the session still useful to members who are not racing the target event?
12. Can the Main Workout remain stable after monthly announcement while pace/group details remain adjustable?

If these questions cannot be answered, the workout is not ready for PLAN.

---

## 15. Participant-facing `Training Effect` communication

The PLAN includes a `Training Effect` column so the purpose of each workout can be explained to members without exposing the full evidence database or coaching logic.

### Role of each PLAN field

- **[Coaching judgment]** `Focus` is a short training-category label such as `Threshold`, `Aerobic Power`, `Speed Endurance`, or `Sharpening`.
- **[Coaching judgment]** `Training Effect` is the participant-facing explanation: **what the workout stimulates → how that can help running**.
- **[Coaching judgment]** `Notes` is reserved for operational context, weather, race proximity, execution cautions, and other session-specific notes. Do not use `Notes` as a second explanation field.

### Writing standard

- **[Coaching judgment]** Keep `Training Effect` to roughly **2–3 short Japanese lines** that can be read aloud before the session or reused in a Strava announcement.
- **[Inference]** Translate the broad evidence-supported adaptation into plain language; do not reproduce scientific terminology merely to sound rigorous.
- **[Evidence-based]** Describe likely training qualities rather than claiming one exact workout guarantees a specific adaptation or race result.
- **[Coaching judgment]** Participant-facing copy does not need citations. Citations and evidence strength live in `knowledge/evidence.md`.
- **[Coaching judgment]** Avoid unsupported numerical promises or oversimplified physiology such as “VO2maxが○%上がる,” “乳酸を除去する,” or “この練習で必ず速くなる.”
- **[Coaching judgment]** Do not justify an exact rep count, recovery, or pace by saying that science proves that exact prescription.

### Default sentence pattern

```text
<何を刺激する練習か>。
<それが走りにどうつながるか>。
```

The wording should describe the **primary intended stimulus**, not every possible adaptation from the workout.

### Participant-facing examples

#### Threshold / Tempo

```text
やや高い強度を長く保つ力を鍛える練習。
速めのペースでも余裕を保ち、後半まで崩れにくい走りにつなげます。
```

#### Aerobic Power / VO2

```text
高い酸素摂取が必要な強度で繰り返し走る練習。
速いペースを有酸素で支える力を刺激し、スピードの余裕度を高めることを狙います。
```

#### 1 km / Speed Endurance

```text
1km前後の速いペースを、疲れても維持する力を狙う練習。
スピードそのものだけでなく、速さを最後まで保つ力を磨きます。
```

#### Short Speed / Neuromuscular

```text
短い時間を速く、フォームを崩さず走る練習。
脚の回転や動きのキレを刺激し、速い動きをスムーズに出す感覚を作ります。
```

#### Hills

```text
上りを使って心肺と脚への負荷を同時に高める練習。
平地とは違う形で、走るためのパワーと強さを刺激します。
```

#### Marathon-oriented controlled work

```text
長めの時間をコントロールして走り続ける練習。
無理に上げすぎず、一定の速いペースを長く維持する力を磨きます。
```

#### Pre-race Sharpening

```text
レース前に短く速い動きを入れて、スピード感を整える練習。
疲労を増やしすぎず、速いペースへの感覚を残すことを狙います。
```

### Final communication check

Before filling `Training Effect`, ask:

1. Can a runner understand it without knowing VO2max, lactate terminology, or periodization theory?
2. Does it explain both **what is being trained** and **why that matters**?
3. Is it consistent with the evidence boundary in `evidence.md`?
4. Would it still be true if the exact rep count or pace range were adjusted slightly on the day?

If the answer to any item is no, rewrite the explanation before publishing the monthly PLAN.
