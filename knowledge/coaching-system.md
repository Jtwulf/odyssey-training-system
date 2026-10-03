# Odyssey Coaching System

Last updated: 2026-10-03

This file translates the routed Evidence Base into operating rules for Odyssey Running's Tuesday Quality Session.

Every meaningful rule uses one of three labels:

- **[Evidence-based]** — directly supported by reasonably applicable research.
- **[Inference]** — a reasonable translation of research into Odyssey's constraints, but not directly tested in this exact setting.
- **[Coaching judgment]** — an operational choice required to run the session; it must not be presented as uniquely proven by research.

Detailed evidence starts at `knowledge/evidence.md`. Google Sheets formatting and maintenance rules live in `knowledge/plan-operations.md`.

---

## 1. System boundary and Source of Truth

### Scope

- **[Coaching judgment]** Odyssey manages the Tuesday **20:00–21:00 Quality Session / Point Workout**.
- **[Coaching judgment]** Typical attendance is **5–10 runners** with a wide ability range.
- **[Coaching judgment]** Planning is displayed in **calendar-month units**, while training logic remains milestone- and progression-aware.
- **[Coaching judgment]** Primary venues through the current cycle are **Yoyogi Park** and **Meiji Jingu Gaien**.

### Non-scope

- **[Coaching judgment]** Do not manage each participant's weekly mileage, sleep, fatigue, injury history, Strava history, or individual weekly plan.
- **[Coaching judgment]** Do not build or maintain an Odyssey participant-performance database merely to assign runners to A/B/C/D groups.
- **[Coaching judgment]** Do not import Justin's personal JTBC training state or personal race targets.
- **[Inference]** Whole-program concepts such as polarized/pyramidal TID are context, not Tuesday-only targets, because Odyssey controls one session per week.

### Source of Truth

```text
GitHub
= WHY / HOW
= Evidence + Coaching Logic + persistent PLAN operating rules

Google Sheets
= WHAT / WHEN
= actual monthly Workout Plan

Strava
= public participant announcement
```

- **[Coaching judgment]** Never duplicate monthly PLAN rows into GitHub.
- **[Coaching judgment]** Future-facing corrections must be persisted in the relevant GitHub rule/evidence file rather than left only in chat memory.

---

## 2. Evidence retrieval protocol

Before designing or materially revising a month:

1. read `knowledge/evidence.md`;
2. identify the next milestone and proposed workout families;
3. read only the routed topic files needed for that problem;
4. separate supported claim, Odyssey inference, and exact coaching prescription;
5. read `plan-operations.md` before editing the Sheet;
6. re-read affected GitHub files and PLAN cells after writing.

### Typical routing

#### 1 km / middle-distance

- `evidence/intensity-domains.md`
- `evidence/threshold-aerobic-power.md`
- `evidence/interval-programming-recovery.md`
- `evidence/speed-economy-hills-warmup.md`
- 1-km sections of `evidence/race-demands.md`
- `evidence/taper-environment.md`

#### Marathon-oriented

- `evidence/training-distribution-periodization.md`
- `evidence/intensity-domains.md`
- `evidence/threshold-aerobic-power.md`
- `evidence/durability-marathon.md`
- marathon section of `evidence/race-demands.md`
- `evidence/taper-environment.md`

Do not load `references.md` unless verifying or changing a claim.

---

## 3. Core design principles

1. **[Evidence-based]** Quality training should not be reduced to one intensity. Threshold, aerobic power, speed, hills, and race-specific stimuli can all have roles.
2. **[Inference]** The objective is a **comparable session-purpose stimulus** appropriate to each group. Identical distance does not imply identical physiological strain because pace and work duration still differ by group.
3. **[Evidence-based]** Interval response depends on intensity, work duration/distance, cumulative work, recovery, environment, and training status. No universal optimal combination exists.
4. **[Coaching judgment]** Exact reps, rest, pace bands, and groups are chosen for the milestone, venue, 60-minute window, and available field data.
5. **[Evidence-based]** Acute response, chronic adaptation, and race performance are separate evidence layers.
6. **[Evidence-based]** Specificity generally increases toward an important event; taper evidence supports lower volume with some retained intensity.
7. **[Coaching judgment]** Progression does not mean harder every Tuesday. It may mean more specificity, better control, different stimulus, deliberate unloading, or lower fatigue cost.
8. **[Evidence-based]** Heat/environment change relative strain at a fixed pace.
9. **[Coaching judgment]** Easy/social running is not the main Tuesday workout; easy running is used for warm-up, recovery, and cooldown.
10. **[Coaching judgment]** For interval-format sessions, prescribe the work by **distance** and keep the repetition distance common across A/B/C/D whenever practical. Use pace, repetition count, and recovery to keep the dose appropriate.

---

## 4. Monthly planning method

For each calendar month, design all Tuesdays together before announcement.

### Step A — identify milestones

Current milestones:

- **2026-09-19 — DESCENTE 1 km Time Trial**
- **2026-11-01 — Seoul Marathon**

### Step B — define the month-level training problem

- **[Inference]** Decide which qualities need emphasis based on the next milestone while retaining value for non-participants.
- Candidate qualities: threshold speed, aerobic power, speed endurance, short speed, hills, race rhythm, sustained tempo, durability-oriented work.

### Step C — assign one primary purpose to each Tuesday

- **[Coaching judgment]** Each session has one primary `Focus`.
- **[Coaching judgment]** Choose the purpose before the workout format; do not choose a familiar workout and invent a reason afterward.

### Step D — select the work unit and dose

For interval-format sessions:

- choose a practical **distance-based repetition** first;
- keep the repetition distance the same across A/B/C/D whenever practical;
- adjust group dose primarily through pace and, when needed, repetition count;
- treat recovery as an independent variable that may be time- or distance-based.

Continuous tempo / steady / sustained continuous work may remain time-based or route-distance-based because uninterrupted duration can be part of the purpose.

Explicitly answer:

- If this is an interval-format session, what common repetition distance is being used?
- What is the expected rep duration for every group?
- What cumulative quality distance/time does every group receive?
- Does any group need fewer repetitions to keep the dose appropriate?
- What must recovery accomplish?

### Step E — check sequence and fatigue

- **[Evidence-based]** Increase event relevance as appropriate and reduce load near competition.
- **[Inference]** Four days before a 1-km TT, prioritize readiness and movement quality over a large training load.
- **[Coaching judgment]** Exact low-volume sharpening remains a coaching prescription.

### Step F — check scope and 60 minutes

- **[Coaching judgment]** The entire session, including transitions, must fit 20:00–21:00.
- **[Coaching judgment]** Do not assume the participants' other six training days.

---

## 5. Standard 60-minute architecture

### Default

```text
20:00–20:10/12  Easy running
20:10/12–20:16/18  Dynamic preparation
20:16/18–20:20  Optional progressive strides / workout-specific prep
~20:20–20:48/50  Main workout
~20:48/50–20:58  Easy cooldown
20:58–21:00  Finish / regroup
```

### Evidence boundary

- **[Evidence-based]** Warming up generally improves subsequent performance.
- **[Evidence-based]** Dynamic preparation often supports sprint/jump readiness; prolonged static-only stretching can impair explosive performance in some contexts.
- **[Evidence-based]** Running-economy evidence does not show a clear acute benefit or harm from any stretching type overall; certainty is low.
- **[Inference]** Easy running → dynamic preparation → progressive strides is a practical speed progression for faster sessions.
- **[Coaching judgment]** Exact minutes, drills, and stride count are not uniquely proven.

### Workout-specific preparation

#### Threshold / controlled tempo

- 10–12 min easy running;
- short dynamic preparation;
- 0–3 progressive strides depending on conditions and starting pace.

#### Aerobic power / 1 km / speed endurance

- 10–12 min easy running;
- dynamic preparation;
- 2–4 progressive strides/controlled accelerations.

#### Hills / short speed

- 10–12 min easy running;
- dynamic preparation;
- progressive accelerations before near-maximal work.

### Cooldown

- Default 7–10 min easy where logistics allow.
- Preserve the one-hour finish; cooldown does not justify overrunning.

---

## 6. Intensity translation

### Common language

- **Moderate / below first threshold:** easy/conversational.
- **Heavy:** controlled sustained work between first threshold and CS, depending on the marker used.
- **CS / heavy-severe boundary:** useful field concept, not mandatory testing for every participant.
- **Severe:** above CS; commonly relevant to aerobic-power and shorter-race work.
- **MAV/vVO2max:** test-specific speed associated with maximal oxygen uptake, not interchangeable with CS or race pace.
- **Extreme/sprint:** very short maximal demand; distinct from relaxed strides or controlled speed endurance.

### Rules

- **[Evidence-based]** LT, VT, CS, HRV thresholds, and race paces are related but not numerically interchangeable.
- **[Coaching judgment]** Use pace ranges plus effort/execution cues rather than false precision.
- **[Coaching judgment]** In heat, fatigue, wind, hills, or congestion, preserve the relative session purpose rather than nominal pace.

---

## 7. pace-group system

### Purpose and participant choice

- **[Coaching judgment]** A/B/C/D are **Workout Target Groups**: simple pace options for the session, not permanent runner rankings or organizer-assigned classifications.
- **[Coaching judgment]** Odyssey publishes the A/B/C/D target pace or split for each workout; participants choose the band that best matches the actual prescribed pace, the day's workout, and their condition.
- **[Coaching judgment]** A participant's usual group identity must not override the actual pace. A runner may choose any band that is appropriate on that day without special administrative handling.
- **[Coaching judgment]** The organizer does not maintain individual performance records or pre-assign each runner to a group before every session.
- **[Coaching judgment]** The main design priority is a clear, sustainable group operation. Physiological comparability should be improved within that constraint rather than by adding participant-data management.
- **[Coaching judgment]** Sex is not a grouping criterion; all four bands are available to any participant.
- **[Coaching judgment]** Pace order is always **A fastest → B → C → D**.

### Internal performance-level reference

These are rough operating images, not hard boundaries and not automatic classifications:

- **Group A:** approximately marathon **2:30 to 2:45 level**; the fastest / sub-elite-oriented workout option.
- **Group B:** approximately **sub-3 marathon target level**; centered on runners aiming to break 3:00 rather than using 2:50 as a lower-bound definition.
- **Group C:** approximately marathon **3:20 to 3:40 level**, with **around 3:30** as the rough internal center.
- **Group D:** approximately **sub-4 to 4:30 marathon level**.

These marathon references are **not normally shown in participant announcements or PLAN pace cells**. They are internal context and may be used to answer a participant who asks which band is likely to suit them. The actual workout pace/split remains the primary selection cue.

The references are deliberately approximate. Small gaps or overlaps are acceptable, and marathon ability is not a complete predictor of short-distance speed, threshold speed, or performance on every workout family.

### Pace-band design

- **[Coaching judgment]** Design the actual A/B/C/D pace from the **purpose and demand of the workout first**. Do not mechanically derive every workout pace from marathon time.
- **[Coaching judgment]** Marathon-level references may be used as a sanity check or rough anchor, but the workout target determines the final band.
- **[Coaching judgment]** Current Odyssey field calibration and the existing PLAN pace bands are important reasonableness checks. If a theory- or formula-driven recalculation produces a large departure from a pace that has otherwise been operating plausibly, re-examine the assumptions and field context before changing the PLAN rather than replacing it automatically.
- **[Coaching judgment]** When migrating existing three-group workouts into the four-group system, preserve the prior operating calibration by mapping **old A → new B, old B → new C, old C → new D**, then design the new Group A target from the workout purpose and the faster performance-level reference.
- **[Coaching judgment]** Keep bands narrow enough to remain meaningful but wide enough to be usable by a mixed-ability group.
- **[Coaching judgment]** Group A should stay within about a **10 sec/km maximum range**.
- **[Coaching judgment]** Group B should stay within about a **10 sec/km maximum range** where practical.
- **[Coaching judgment]** Group C should preferably stay near a **10 sec/km range** and should normally remain within about **15 sec/km maximum**.
- **[Coaching judgment]** Group D should use the **sub-4 to 4:30 marathon-level reference** only as a rough reasonableness check, then publish roughly a **10–20 sec/km practical range** appropriate to the workout. Treat about **20 sec/km as the normal maximum** rather than expanding the band indefinitely to cover every slower runner.
- **[Coaching judgment]** Group D is intended to remain usable across roughly the **sub-4 to 4:30 marathon level** where practical, but the published pace band does not need to become so wide that it loses its training meaning.
- **[Coaching judgment]** Gaps between A/B/C/D pace ranges are acceptable. The four bands do not need to form a continuous pace ladder because participants self-select the most appropriate actual pace.
- **[Coaching judgment]** Round published per-kilometer pace targets to practical **5 sec/km increments**.
- **[Coaching judgment]** Do not add special D-only participant-facing wording by default. Keep PLAN and announcement presentation consistent across A/B/C/D; use normal on-the-day coaching when someone falls outside the published band.
- **[Coaching judgment]** Published ranges are guidance, not a requirement to force every runner to hit the same exact pace. Conditions, current feel, and execution quality may justify modest on-the-day adjustment.

### Group-specific dose adjustment

- **[Coaching judgment]** In interval-format sessions, keep the repetition distance common across A/B/C/D whenever practical and change **repetition count before repetition distance** when one group would otherwise receive excessive total work.
- **[Coaching judgment]** Group D may complete fewer repetitions when its longer repetition time, current load, or session-time requirement would otherwise create excessive total quality duration or fatigue.
- **[Coaching judgment]** Group-specific repetition reductions should normally be a **Group D tool**. Keep A, B, and C on the same repetition count when practical rather than routinely creating separate A/B/C volumes.
- **[Coaching judgment]** A group-specific repetition distance is an exception, not a normal dose-control tool. Use it only when a common distance would materially distort the workout purpose, violate the 60-minute window, or create a safety/logistics problem, and document the reason.
- **[Coaching judgment]** Do not add a Group E by default. If participation demand below the current D coverage becomes material in practice, reconsider the group system deliberately rather than pre-emptively adding complexity.

### Pace-setting hierarchy for the published bands

1. the physiological/race-specific purpose of the session;
2. relevant Odyssey field calibration from similar sessions;
3. broad performance-level references as a reasonableness check;
4. conservative adjustment for uncertainty, environment, and group logistics.

Do not collect participant data solely to run this hierarchy. It is used to design useful public A/B/C/D options, not to score or classify individuals.

### Display

- Normally show pace ranges, not a single second per kilometer.
- The **per-kilometer pace is the primary reference** whenever it is meaningful.
- For distance repetitions, also show a practical rep split as a reference while retaining the corresponding `/km` pace. The split may use one-second precision when helpful even though `/km` targets are rounded to 5-second increments.
- For short work, effort/rhythm may supplement pace, but do not omit a meaningful `/km` pace merely because a split is shown.
- Do not normally add marathon-time labels such as `2:30–2:45`, `Sub-3`, or `Sub-4` to participant announcements or PLAN group headings. If a participant asks which band may suit them, these references can be explained verbally as rough guidance.

### Environment and day-of calibration

- **[Evidence-based]** Heat, humidity, wind, surface, and congestion can change the relative strain of a fixed pace.
- **[Coaching judgment]** Do not require the baseline PLAN pace to be pre-adjusted from Tokyo historical-average temperature or a fixed seasonal penalty table.
- **[Coaching judgment]** Keep the planned target as the baseline and make the smallest necessary adjustment on the day when actual conditions materially change the intended stimulus. Use the heat/environment hierarchy in Section 12.

### Current field calibration — not a permanent pace table

- 2-km repetitions, 2-min rest: fastest ~3:40–3:50/km; next ~4:10/km; slower ~5:00/km.
- 1-km repetitions: fastest ~3:30/km; next ~3:40–3:50/km; next ~4:20–4:30/km.

These observations predate the four-group expansion and are field references, not a direct A/B/C/D mapping. Recalibrate the published bands from actual Odyssey execution and the purpose of the session. Current PLAN pace bands are working estimates rather than fixed universal values.

---

## 8. Workout design matrix

Exact values are coaching judgments. The matrix identifies the primary target and the variables that should dominate the decision.

| Workout family | Primary target | Expected transfer | Work-unit tendency | Recovery objective | Main fatigue risk | Evidence route |
|---|---|---|---|---|---|---|
| Continuous tempo | uninterrupted controlled high aerobic output | sustained pace/rhythm | usually time or route distance | none | drifting above target and fading | THR-001/002 |
| Cruise intervals | controlled threshold-oriented quality volume | sustainable speed and pace control | distance-based repetitions | short continuity-preserving recovery | becoming severe-domain intervals | THR-001/002, REC-002 |
| Aerobic power | sustained severe-domain high oxygen-uptake work | VO2max/MAV support and faster-pace reserve | distance-based repetitions selected with expected rep duration in mind | preserve work quality with incomplete/appropriate recovery | chasing maximal pace or excess volume | AP-001–004 |
| 1-km race rhythm | distance-specific rhythm and split judgement | specificity and pacing | distance-based repetitions | enough recovery for target rhythm | turning into repeated all-out trials | RACE-1K-001/002, IP-003 |
| Speed endurance | maintain fast running under controlled accumulating fatigue | sustain speed late in short race | distance-based repetitions | balance quality and fatigue accumulation | mechanics collapse / excessive anaerobic load | SPD-001, RACE-1K-001 |
| Short speed | fast mechanics and speed reserve | movement quality and speed access | short distance-based repetitions | generous recovery | confusing with exhausting SIT | SPD-001, NM-001 |
| Hills — long | aerobic + muscular overload | high aerobic demand and force-oriented running | fixed hill distance / segment | preserve repeatability; account for downhill | calf/Achilles/muscular load | HILL-001 |
| Hills — short | acceleration/force/power | neuromuscular/power stimulus | short distance | walk/jog-back or generous recovery | maximal work without preparation | HILL-001, NM-001 |
| Marathon-oriented controlled | sustainable speed and fatigue resistance | threshold/durability support | longer time/distance | short recovery or continuous | assuming Tuesday replaces long-run/volume | DUR-001–004, MAR-001/002 |
| Sharpening | readiness and fast rhythm with low fatigue | race-day movement familiarity | short race-relevant distance | generous recovery | trying to create fitness days before race | TAP-001/002 |

---

## 9. Distance-first rule for interval-format work

The scientific evidence does **not** establish distance-based prescription as physiologically superior to time-based prescription. This section is an Odyssey **operating rule** chosen for participant comprehension and field execution.

### Interval-format default

- **[Coaching judgment]** A workout made of repeated work bouts separated by recovery is prescribed by **distance**.
- **[Coaching judgment]** This applies to cruise/threshold intervals, aerobic-power intervals, race-rhythm repetitions, speed endurance, short speed, hill repetitions, and sharpening.
- **[Coaching judgment]** Continuous tempo, steady, or other uninterrupted sustained running is not treated as interval-format work for this rule and may remain time-based or route-distance-based.
- **[Coaching judgment]** Recovery units are independent from work units. A distance-based repetition may use a time-based recovery, jog-back distance, standing recovery, or another recovery format that serves the next repetition.

### Common distance across pace groups

- **[Coaching judgment]** Keep the **repetition distance the same across A/B/C/D whenever practical** so participants can easily understand what they are running and compare repetitions.
- **[Coaching judgment]** Adjust the workout first through group pace and, when needed, repetition count. Group D is normally the first place to reduce repetitions when slower rep duration would otherwise create excessive total work.
- **[Coaching judgment]** Different repetition distances between groups are an exception. Use them only when a common distance would materially distort the intended stimulus, exceed the 60-minute session window, or create a meaningful safety/venue/logistics problem.

### Evidence boundary

- **[Evidence-based]** Work-bout duration remains an important dose variable, so the same distance can produce materially different acute demands across groups.
- **[Inference]** A common distance improves operational clarity; it does not prove equal physiological stimulus.
- **[Coaching judgment]** Therefore every interval design still checks expected rep duration, cumulative quality dose, pace decay, and recovery before approval.

---

## 10. Recovery design

- **[Evidence-based]** Active recovery is not universally superior to passive recovery.
- **[Coaching judgment]** Select recovery according to the desired next repetition.

### Practical inference

- Threshold/cruise: short easy jog often preserves continuity.
- Aerobic power: enough recovery to preserve multi-minute work quality without unintended full reset when cumulative aerobic strain is desired.
- Speed endurance: sufficient recovery to control speed decay and mechanics.
- Short speed: longer/passive/walk-back can preserve velocity and technique.
- Sharpening: generous walk-jog/passive recovery protects low fatigue.

Exact durations must fit the 60-minute window.

---

## 11. Durability and marathon logic

- **[Evidence-based]** Durability is resistance to physiological/performance deterioration during/after prolonged exercise and is associated with marathon performance.
- **[Evidence-based]** Direct evidence identifying the best durability intervention is incomplete.
- **[Inference]** Sustained tempo, longer controlled intervals, whole-program volume/long runs, and race-specific work may contribute, but Odyssey controls only Tuesday.
- **[Coaching judgment]** Do not label every long/hard workout “durability.” The primary target must be maintaining quality under controlled sustained fatigue.
- **[Coaching judgment]** After the 1-km milestone, increase sustained/threshold/marathon relevance selectively without eliminating aerobic-power, hill, or speed tools.

---

## 12. Environment and venue logic

### Heat/environment

- **[Evidence-based]** Heat/humidity increase strain and can reduce sustainable running performance.
- **[Inference]** Pace, groups, recovery, and group-specific volume may need adjustment to preserve the target.
- **[Coaching judgment]** No fixed seconds-per-kilometer heat penalty.

Adjustment hierarchy:

1. reduce target pace / use effort cue;
2. widen pace range or change group assignment;
3. modestly extend recovery when repeat quality is primary;
4. shorten one group or final reps;
5. adjust warm-up/water/shade;
6. structurally change/cancel only for safety/logistics.

### Yoyogi Park

Available characteristics:

- ~1-km usable section;
- ~2-km loop;
- ~100-m hill.

Select the section based on purpose; do not build a detailed GPS database without need.

### Meiji Jingu Gaien

Representative loop: **~1.325 km**.

Known format:

```text
1 km hard
+ remaining ~300–325 m jog
= one loop
```

Operationally simple, but faster/slower groups receive different work and recovery durations. Use time-based recovery or alternative regrouping when comparable duration matters.

---

## 13. Announcement stability

Once a calendar month's plan has been announced:

- preserve the Main Workout structure unless safety/logistics or an explicitly approved coaching reason requires change;
- allowable adjustments include pace, assignment, heat response, modest recovery change, and shortening one group;
- avoid changing an announced `1 km × 5` into an unrelated `400 m × 12` casually.

This is an operational commitment, not a scientific claim.

---

## 14. Current milestone logic

### 2026-09-19 DESCENTE 1 km Time Trial

- **[Evidence-based]** Approximately 1 km has substantial aerobic and anaerobic demand.
- **[Inference]** Preparation should combine threshold support, aerobic power, distance/rhythm-specific speed endurance, and low-volume sharpening rather than repeated all-out 1-km trials.
- **[Evidence-based]** Taper principle: lower load with retained intensity.
- **[Inference]** 9/15 should preserve rhythm/readiness with low residual fatigue.
- **[Coaching judgment]** Exact sessions remain in Google Sheets.

### 2026-11-01 Seoul Marathon

- **[Evidence-based]** Marathon performance depends on whole-program volume, sustainable speed/economy, long-run/race-specific exposure, and durability.
- **[Inference]** After 9/19, Tuesday can shift toward longer controlled work and sustained quality.
- **[Coaching judgment]** Sessions remain useful to non-Seoul runners; Odyssey does not provide the complete marathon program.

---

## 15. Historical Odyssey sessions — field calibration only

Historical sessions are operational context, not proof of optimality.

### 2026-06-09 — Intervals.icu `i155686940`

- Oda Field; `800 m × 6`.
- Fast side approximately 3:10/km by user report.
- User report takes priority over unreliable automatic split interpretation.

### 2026-07-14 — `i165991824`

- Yoyogi; `20 min pace run / tempo`.
- Approx. fast 3:50/km; B ~4:30/km.
- Operationally a good Yoyogi fit.

### 2026-07-21 — `i167711146`

- Gaien; `1 km × 4`.
- Fast side approximately 3:40/km.
- Recovery = remaining ~300–325 m jog.
- Operationally easy to run.

### 2026-08-04 — `i172341372`

- Yoyogi; ~100-m hill dash ×15.
- Useful occasionally, not as a frequent default.

### Explicit exclusions

- 2026-08-11 — not Odyssey.
- 2026-08-18 `i177181493` — not Odyssey.
- 2026-07-07 — not confirmed.

---

## 16. Claims the system must never make

Do not claim:

- “1 km × 4 with 2 min recovery is scientifically optimal.”
- “Group A must always run 3:40/km.”
- “Active recovery is always better.”
- “Polarized training proves Tuesday should be VO2 every week.”
- “Everyone should run the same distance for the same stimulus.”
- “Four Tuesdays form a scientifically mandatory block.”
- “More time near VO2max guarantees better race performance.”
- “This one session improves durability.”
- “Heat requires exactly X seconds/km reduction.”

Use:

```text
Evidence says: <supported broad principle>
Inference says: <how it applies to this milestone/group/venue>
Coaching judgment says: <exact prescription>
```

---

## 17. Design quality check

For each Tuesday verify:

1. Primary training target?
2. Relevant Evidence Claim IDs?
3. Expected transfer to running?
4. Acute versus chronic versus performance evidence separated?
5. For interval-format work, is the repetition distance distance-based and common across groups? If not, is the exception justified? For continuous work, is time or route distance appropriate to the purpose?
6. Expected work duration and cumulative dose for every group?
7. Recovery purpose?
8. Pace bands make sense for the workout purpose and broad A/B/C/D ability references rather than aspiration alone?
9. Venue and environment preserve or distort the target?
10. Full session fits 20:00–21:00?
11. Sequence and race proximity justify fatigue cost?
12. Useful to non-participants?
13. Main structure stable after announcement?
14. Training Effect remains true after modest day-of adjustment?

If these cannot be answered, the workout is not ready for PLAN.

---

## 18. Participant-facing `Training Effect`

`Training Effect` explains:

```text
<何を刺激する練習か>。
<それが走りにどうつながるか>。
```

Rules:

- 2–3 short Japanese lines;
- plain language;
- describe the intended quality, not every possible adaptation;
- no citations in PLAN;
- no guaranteed result or unsupported numerical promise;
- no oversimplifications such as “乳酸を除去する” or “必ずVO2maxが上がる”;
- exact rep count/rest must not be described as scientifically unique.

Examples:

### Threshold

```text
やや高い強度を長く保つ力を鍛える練習。
速めのペースでも余裕を保ち、後半まで崩れにくい走りにつなげます。
```

### Aerobic Power

```text
高い酸素摂取が必要な強度を繰り返し走る練習。
速いペースを有酸素で支える力と、スピードの余裕度を刺激します。
```

### 1 km Speed Endurance

```text
1kmに近い速いリズムを、疲れても維持する力を狙う練習。
スピードだけでなく、その速さを最後まで保つ力を磨きます。
```

### Durability-oriented sustained work

```text
長めの時間をコントロールして走り、疲れてきてもペースとフォームを保つ練習。
長距離レースの後半でも走りを崩しにくくする土台を狙います。
```

### Sharpening

```text
レース前に短く速い動きを入れて、スピード感を整える練習。
疲労を増やしすぎず、速いペースへの感覚を残します。
```
