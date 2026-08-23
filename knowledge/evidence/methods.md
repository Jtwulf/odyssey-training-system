# Evidence Methods and Claim Schema

Last reviewed: 2026-08-23

This file defines how Odyssey Training System evaluates, stores, and retrieves scientific evidence. It is a pragmatic operating framework, not a substitute for a formal GRADE assessment.

---

## 1. Scope boundary

The evidence layer answers:

- what training quality or response is supported;
- which outcomes were measured;
- in which population and context;
- how strong and directly applicable the evidence is;
- which programming variables appear material;
- what the evidence does **not** establish.

The evidence layer does **not** decide an Odyssey calendar date, exact repetition count, exact pace band, exact recovery, or group assignment. Those are translations performed in `knowledge/coaching-system.md` and recorded as actual sessions in Google Sheets `PLAN`.

---

## 2. Source hierarchy

Use sources in this order where available:

1. systematic review / meta-analysis;
2. consensus or position statement;
3. randomized or controlled intervention;
4. peer-reviewed original study;
5. high-quality scientific/practice review;
6. coaching inference only where direct evidence is insufficient.

General blogs, commercial training articles, social-media posts, and unsourced coaching claims are not primary evidence.

A newer publication does not automatically outrank an older one. Study design, population, outcome, risk of bias, consistency, and directness all matter.

---

## 3. Outcome-type convention

Every important claim should identify which type of outcome supports it.

### Acute response

What happens within one session or immediately after it, for example:

- time at or near VO2max;
- blood lactate;
- oxygen uptake kinetics;
- heart rate or RPE;
- mechanics or speed decrement.

An acute response is a mechanistic indicator. It is **not automatically evidence of superior chronic adaptation or race performance**.

### Chronic adaptation

What changes after a multi-week intervention, for example:

- VO2max / VO2peak;
- critical speed or threshold speed;
- running economy;
- sprint ability;
- physiological durability.

### Performance outcome

A directly performance-relevant result, for example:

- time trial;
- race time;
- time to exhaustion;
- maximal aerobic speed or power where the study treats it as a performance outcome.

### Observational association

A relationship measured without an intervention. It can identify plausible determinants or real-world patterns but cannot establish causality.

### Practice description

What successful athletes or published plans commonly do. It informs plausibility and context, but successful practice is not proof that the described approach caused success or is optimal.

---

## 4. Evidence-strength rating

Rate the **certainty of the supported claim**, independently from its directness to Odyssey.

### High

Typically:

- a reasonably recent systematic review/meta-analysis;
- several consistent controlled studies;
- an outcome directly matching the claim;
- no major contradiction that changes the conclusion.

### Moderate

Typically:

- a review with heterogeneity, limited trials, or mixed populations;
- several studies with a broadly consistent direction but important uncertainty;
- a strong acute/mechanistic evidence base with less certain long-term transfer.

### Low

Typically:

- one or a few small studies;
- observational or practice-derived evidence;
- substantial methodological inconsistency;
- an indirect population, modality, or outcome;
- a claim requiring meaningful inference beyond the measured result.

Do not average multiple weak studies into a confident statement merely because there are many citations.

---

## 5. Directness-to-Odyssey rating

Rate applicability separately from evidence strength.

### High directness

Most characteristics are close to Odyssey:

- running rather than another modality;
- trained or recreationally trained adult runners;
- a relevant work duration, race distance, or session objective;
- an intervention or acute protocol that resembles a running Quality Session.

### Moderate directness

Some characteristics transfer reasonably but not exactly:

- mixed endurance sports including running and cycling;
- healthy adults with varied training status;
- trained athletes from non-running endurance sports;
- a relevant mechanism but a different session architecture.

### Low directness

Important mismatch exists:

- team-sport repeated sprint evidence applied to distance runners;
- strength or plyometric programs interpreted as proof for a few drills;
- cycling-only evidence used for running prescription;
- elite-only or untrained-only evidence generalized to a mixed community group;
- complete-program evidence used to dictate one Tuesday session.

High-quality evidence can still have low directness. Low directness requires conservative translation.

---

## 6. Required population and context metadata

For each central source or claim, record what is available:

- **Sample:** total `n` and, when reported, female/male distribution;
- **Age:** mean/range or broad adult/youth classification;
- **Training status:** untrained, active, recreationally trained, trained, well-trained, highly trained, elite;
- **Sport / modality:** running, cycling, mixed endurance, team sport, strength training;
- **Design:** systematic review, meta-analysis, crossover, RCT, observational analysis, scientific/practice review;
- **Exposure:** acute protocol or intervention duration and frequency;
- **Outcome:** acute, chronic, performance, observational, or practice description.

When a review contains heterogeneous populations, say so rather than inventing one representative population.

---

## 7. Standard claim format

Use stable claim IDs. Topic prefixes include:

- `DOM` — intensity domains;
- `TID` — training-intensity distribution;
- `PER` — periodization/progression;
- `THR` — threshold/tempo;
- `AP` — aerobic power / VO2 intervals;
- `IP` — interval programming;
- `REC` — recovery;
- `SPD` — sprint/speed endurance;
- `ECO` — running economy / strength;
- `HILL` — uphill running;
- `WU` — warm-up;
- `RACE-*` — event demands;
- `DUR` — durability;
- `MAR` — marathon-oriented training;
- `TAP` — taper;
- `HEAT` — heat/environment.

Recommended structure:

```text
### CLAIM-ID — Short title

Research question
Supported claim
Training target
Expected transfer
Acute evidence
Chronic adaptation evidence
Performance evidence
Programming variables
Population / context
Evidence strength
Directness to Odyssey
Limitations
What this does not prove
Sources
Last reviewed
```

Not every field requires a long paragraph. Use `Not directly tested` where an outcome is absent rather than filling the gap with inference.

---

## 8. Claim-to-source mapping

Use stable source IDs based on PMID whenever available:

```text
PMID-42237396
PMID-38717713
```

Use a DOI-based ID only when no PMID is available:

```text
DOI-10.1371-journal.pone.0282838
```

Each claim lists its supporting source IDs. Full bibliographic and population metadata is stored once in `references.md` to prevent duplication.

A source may support several claims, but every use must remain within what the study measured.

---

## 9. Programming-variable convention

Where relevant, separate these variables instead of treating a workout name as a complete prescription:

- target intensity or intensity domain;
- work-bout duration;
- work distance;
- repetitions and sets;
- cumulative quality duration/distance;
- recovery duration;
- recovery mode: jog, walk-jog, passive/standing, none;
- work-to-recovery relationship;
- within-repetition intensity pattern;
- session frequency and intervention duration;
- venue, gradient, surface, temperature, and humidity.

Evidence rarely identifies a single universally optimal combination. Exact Odyssey prescriptions remain coaching judgments constrained by these variables.

---

## 10. Language and inference rules

Use calibrated wording:

- `supports`, `is associated with`, `can improve`, `appears useful`, `did not establish`;
- avoid `proves`, `guarantees`, `always`, `must`, or `optimal` unless the evidence genuinely supports that scope.

Do not convert:

- acute time near VO2max into guaranteed race improvement;
- an association into causality;
- a mean group response into a universal individual response;
- a multi-week strength program into proof for one drill sequence;
- whole-program TID into a fixed rule for Tuesday;
- a race-distance average into a precise pace for every runner.

---

## 11. Context-efficient retrieval

`knowledge/evidence.md` is the routing index. Monthly planning should load only the topic files relevant to the current milestone and workout families.

Examples:

### 1 km-oriented month

Read:

- `intensity-domains.md`;
- `threshold-aerobic-power.md`;
- `interval-programming-recovery.md`;
- `speed-economy-hills-warmup.md`;
- `race-demands.md`;
- `taper-environment.md`.

### Marathon-oriented month

Read:

- `training-distribution-periodization.md`;
- `intensity-domains.md`;
- `threshold-aerobic-power.md`;
- `durability-marathon.md`;
- `taper-environment.md`.

Do not load the entire reference registry unless verifying a source or revising the evidence base.

---

## 12. Update and verification workflow

When evidence is added or materially changed:

1. verify title, year, publication, PMID/DOI, study design, and central result from the journal or PubMed record;
2. update `references.md`;
3. update the relevant claim and source mapping;
4. distinguish direct evidence from inference;
5. check whether `coaching-system.md` requires a rule change;
6. re-read all changed files after writing;
7. update the `Last reviewed` date.

Research gaps should remain visible. Missing direct evidence is not a reason to invent precision.