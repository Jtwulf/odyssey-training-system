# Odyssey Evidence Index

Last full evidence review: 2026-08-23

This file is the lightweight entry point to Odyssey Training System's scientific evidence. Detailed claims live in `knowledge/evidence/` topic files. Exact Odyssey prescriptions belong in `knowledge/coaching-system.md`; actual monthly sessions belong only in Google Sheets `PLAN`.

---

## 1. Core evidence principles

1. **Training stimulus, not visual uniformity, is the primary design target.** Equal distance or equal pace does not guarantee equal physiological demand across a heterogeneous group.
2. **Workout names are incomplete prescriptions.** Intensity, work duration/distance, cumulative volume, recovery, environment, and athlete context interact.
3. **Acute response, chronic adaptation, and performance outcome are separate evidence layers.** More time near VO2max in one session does not automatically prove better long-term race performance.
4. **Research generally supports ranges and principles, not one uniquely correct repetition count, recovery, or pace.** Exact prescriptions remain coaching judgments.
5. **Specificity should increase toward important events, while load is managed rather than increased every week.** Taper evidence supports reducing volume while retaining some intensity.
6. **Whole-program evidence must be applied conservatively.** Odyssey manages one Tuesday Quality Session, not each runner's complete week.
7. **Evidence strength and directness to Odyssey are different.** A high-quality cycling or team-sport meta-analysis may have limited directness to mixed-ability distance runners.
8. **Environment changes relative intensity.** Heat, humidity, grade, wind, and congestion can require pace/recovery/volume adjustment to preserve the intended stimulus.
9. **Durability complements fresh-state fitness.** Resistance to physiological/performance decline during prolonged running matters increasingly for longer races, but direct intervention evidence remains incomplete.
10. **Evidence gaps must remain visible.** Missing evidence is not filled with false precision.

---

## 2. Evidence-system files

| File | Primary contents |
|---|---|
| [`evidence/methods.md`](evidence/methods.md) | Evidence strength, directness, outcome types, population metadata, claim schema, retrieval rules |
| [`evidence/references.md`](evidence/references.md) | Verified bibliography and study/population context using stable Source IDs |
| [`evidence/intensity-domains.md`](evidence/intensity-domains.md) | Moderate/heavy/severe/extreme domains, LT/VT/CS/MAV relationships and limits |
| [`evidence/training-distribution-periodization.md`](evidence/training-distribution-periodization.md) | Whole-program TID, progression, specificity, and Tuesday-only scope boundary |
| [`evidence/threshold-aerobic-power.md`](evidence/threshold-aerobic-power.md) | Threshold/tempo, cruise intervals, aerobic-power/VO2 intervals, acute versus chronic transfer |
| [`evidence/interval-programming-recovery.md`](evidence/interval-programming-recovery.md) | Work duration, cumulative dose, time/distance choice, recovery duration/mode, mixed-group dosing |
| [`evidence/speed-economy-hills-warmup.md`](evidence/speed-economy-hills-warmup.md) | Sprint/speed, running economy/strength, neuromuscular stimulus, hills, warm-up/stretching |
| [`evidence/race-demands.md`](evidence/race-demands.md) | 1 km, 3–5 km, 10 km, Half Marathon, and Marathon demands/specificity |
| [`evidence/durability-marathon.md`](evidence/durability-marathon.md) | Durability definition/evidence and the limited role of one Tuesday in marathon preparation |
| [`evidence/taper-environment.md`](evidence/taper-environment.md) | Taper/sharpening, heat acclimatisation, environmental adjustment and evidence boundaries |

---

## 3. Topic routing for monthly planning

Do not load every detailed file by default. Read only what the next milestone and proposed workout families require.

### 1 km / middle-distance-oriented planning

Read:

- `intensity-domains.md`;
- `threshold-aerobic-power.md`;
- `interval-programming-recovery.md`;
- `speed-economy-hills-warmup.md`;
- relevant sections of `race-demands.md`;
- `taper-environment.md`.

### 3–10 km planning

Read:

- `intensity-domains.md`;
- `threshold-aerobic-power.md`;
- `interval-programming-recovery.md`;
- relevant sections of `race-demands.md`;
- `training-distribution-periodization.md`;
- `taper-environment.md` when a race is close or conditions are material.

### Half-marathon / marathon-oriented planning

Read:

- `training-distribution-periodization.md`;
- `intensity-domains.md`;
- `threshold-aerobic-power.md`;
- `durability-marathon.md`;
- relevant sections of `race-demands.md`;
- `taper-environment.md`.

### Hills / short speed / warm-up decisions

Read:

- `speed-economy-hills-warmup.md`;
- `interval-programming-recovery.md`;
- the relevant race-demand section.

Read `references.md` only when verifying, challenging, or updating a claim.

---

## 4. Evidence-strength and directness shorthand

Detailed rules are in `evidence/methods.md`.

### Evidence strength

- **High:** strong review/meta-analytic or consistent controlled evidence for the stated claim.
- **Moderate:** useful evidence with heterogeneity, limited trials, or uncertain transfer.
- **Low:** small/single/observational/indirect evidence or substantial inference.

### Directness to Odyssey

- **High:** running, relevant adult runner population, relevant session or event demand.
- **Moderate:** mixed endurance population/modality or a related but not identical protocol.
- **Low:** substantial population, modality, program-scope, or intervention mismatch.

A claim can be High strength and Low directness.

---

## 5. Claim architecture

Detailed topic files use stable Claim IDs and Source IDs.

Example:

```text
AP-001
= Multi-minute intervals are effective for accumulating high oxygen-uptake time

Sources
= PMID-42237396, PMID-42482078, PMID-39835194, PMID-33826121
```

Each central claim distinguishes where applicable:

- Supported claim;
- Training target;
- Expected transfer;
- Acute evidence;
- Chronic adaptation evidence;
- Performance evidence;
- Programming variables;
- Population / context;
- Evidence strength;
- Directness to Odyssey;
- Limitations;
- What the evidence does not prove.

---

## 6. Current evidence-backed design boundaries

### Supported broadly

- mixed use of threshold, aerobic-power, speed, hills, and race-specific stimuli;
- multi-minute intervals as an effective way to accumulate high oxygen-uptake time;
- work duration as a material programming variable;
- active and passive recovery both being valid depending on purpose;
- warm-up before quality running;
- mixed aerobic/anaerobic demand for 800–1500 m and approximately 1 km;
- high-load/combined strength programs improving running economy over multiple weeks;
- planned progression and increasing specificity;
- reduced volume with retained intensity during taper;
- heat increasing physiological strain and often reducing sustainable performance;
- durability as a meaningful longer-event performance concept.

### Not directly established

- one optimal repetition count, recovery, pace, or work-to-rest ratio;
- one best time-based or distance-based format for mixed groups;
- exact A/B/C/D pace bands;
- a universal warm-up drill sequence;
- one exact 1-km sharpening workout four days before racing;
- a fixed heat pace adjustment;
- the best intervention for improving durability;
- a complete marathon program delivered through one Tuesday session.

---

## 7. Known evidence gaps relevant to Odyssey

1. **Mixed-ability community groups:** little direct research tests one 60-minute session spanning sub-2:50 to approximately sub-4 marathon ability.
2. **Time versus distance:** underlying duration/specificity principles are supported, but direct comparative group-session trials are lacking.
3. **Exact group pace calibration:** evidence supports relative intensity more strongly than universal pace tables.
4. **One-session ownership:** most intervention evidence evaluates several weekly sessions.
5. **1-km-specific training:** direct 1000-m prescription trials are sparse; evidence is triangulated from 800/1500, HIIT, sprint, and taper research.
6. **Durability intervention:** measurement and performance association evidence is ahead of comparative training-intervention evidence.
7. **Female representation:** several threshold, recovery, speed, and durability studies are male-dominant or small.
8. **Outdoor transfer:** treadmill, track, road, hills, heat, and GPS/landmark conditions are not interchangeable.

---

## 8. Evidence-to-PLAN chain

Use this chain for every session:

```text
Evidence claim
→ supported training target / expected transfer
→ Odyssey inference for this milestone and group
→ coaching judgment for exact work, recovery, groups, venue, and timing
→ participant-facing Training Effect
→ actual PLAN row
```

The participant-facing explanation should remain true if a pace range or one group's repetition count is adjusted modestly on the day.

---

## 9. Maintenance rule

When a new study changes a central claim:

1. verify the publication and central result;
2. add/update the Source ID in `references.md`;
3. update the relevant Claim ID;
4. reconsider the Coaching Logic;
5. audit affected future PLAN rows;
6. re-read all written files;
7. update the review date.

Do not expand this index with full study summaries. Detail belongs in the routed topic files.