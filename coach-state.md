# COACH STATE — live training status
*Maintained by the coach. Last updated: October 11, 2026 (after the Sep 16 – Oct 10 backlog was logged)*

**Read this file at the start of every session, together with `workout-log.json`.** It holds current working weights, active decisions, and open questions. Where it disagrees with the skill's reference files, THIS FILE WINS — the reference files (`brandon-profile.md`, `exercise-library.md`) hold slow-changing background (meals, injury history, preferences) and their weight tables are stale as of June. This file holds the live state.

---

## PROGRAM — FAT LOSS PHASE, starts Oct 12 2026

**Brandon's stated goal (Oct 11): lose belly fat accumulated over three months of travel, MAINTAIN STRENGTH, 4 gym days a week. He does not want to use the scale.**

### The governing principle — do not get this backwards
**The lifting is not the fat-loss tool. It is the muscle-protection tool.** Four sessions burn roughly 1,600–2,000 kcal a week. A 500 kcal/day food change is 3,500. Food is the lever by a factor of two, and it is the more reliable one.

So **do NOT convert his lifting into circuits, high-rep "metabolic" work, or anything that sacrifices load.** That is the standard mistake and it would cost him the exact thing he said he wants to keep. Heavy compounds in a calorie deficit, plus high protein, are what preserve lean mass. The deficit comes from the kitchen; cardio tops it up.

### Session architecture (all four days)
1. **Block 1 — two heavy compounds.** 3–4 × 6–8, full 2–3 min rest. **Untouched by the fat-loss goal.** This is the strength insurance.
2. **Block 2 — accessories PAIRED as supersets.** 45–60 sec between pairs instead of 90 straight. Same volume, ~30% less time, higher average heart rate. This is where the fat-loss adjustment lives.
3. **Block 3 — core circuit**, rotated.
4. **Finisher — 12–15 min incline walk. NON-NEGOTIABLE in this phase.** He skips it when sessions run long; in a deficit phase it stays.

### 4-day rotation — both lower days hinge AND squat, both upper days push AND pull
Frequency matters more than specialization for holding strength in a deficit, so every muscle group gets hit twice a week. The days only flip which movement leads.

| Day | Focus | Leads with |
|-----|-------|-----------|
| **A — Lower** | Squat emphasis | Barbell squat primary, hinge secondary |
| **B — Upper** | Press emphasis | DB shoulder press (permanent lead), DB bench second |
| **C — Lower** | Hinge emphasis | Barbell deadlift primary, machine squat/lunge secondary |
| **D — Upper** | Pull emphasis | Row primary, pulldown second, pressing after |

Hip thrust machine runs on Day A (he asked for it back, every other lower day). Free weights first throughout, per his stated preference.

### Cardio and steps
- **2 × 35–45 min Zone 2 on off days** — bike, elliptical or incline walk. Conversational the whole time. He liked this format in August.
- **8–10k steps daily floor.** He hit 15–20k on NYC walking days without trying.
- Zone 2 only. Do not program HIIT on top of four lifting days in a deficit — recovery is the limiting factor, and he already has a scapula with three strains in it.

### Nutrition — THIS IS THE ACTUAL PROJECT
**Targets already on file: 1,900 kcal/day, 140 g protein. Untracked since May 17 — five months.**

**DIAGNOSED Oct 11: nothing is broken.** Both GitHub syncs share one token (`WorkoutLogSync._headers` calls `GitHubSync.getToken()`), and his workout-log pushes have been landing fine — so the token is valid and the push path works. `fitness-data.json` has not updated because **he simply has not pressed "Save Day" on the nutrition tab since May 17.** He kept logging workouts and stopped logging food.

**Brandon chose (Oct 11) to resume tracking in the app.** So the fix is behavioral, not technical: start pressing Save Day. One caveat in the code worth knowing — `GitHubSync.push` opens with `if(!token) return;`, which fails **silently**, while `WorkoutLogSync.push` toasts a warning. If nutrition data ever stops again with no visible error, that silent return is the first suspect.
- **Protein 140 g is the non-negotiable number** — it is what makes the deficit cost fat instead of muscle.
- **Alcohol is the first cut.** He named it himself as elevated through the travel stretch.
- Expect the first 2–3 weeks to show faster visible change than the real fat loss rate, because travel bloat, water and inflammation clear first. Do not let him over-read that, or under-read the slowdown after.

### Measurement — NO SCALE, but WEEKLY WAIST TAPE (his choice, Oct 11)
- **NO SCALE — he does not want to weigh himself. Do not ask for weight, do not ask him to reconsider.**
- **Waist at the navel, once a week.** He offered this himself after initially declining. It is the primary number and it is literally the thing he is trying to change.
- **Protocol matters more than the number** — an inconsistent measurement is worse than none:
  - Same morning each week, before eating or drinking
  - Level with the navel, tape parallel to the floor all the way around
  - **At the end of a normal exhale. Not sucked in, not pushed out.**
  - Snug against skin without compressing it
  - Record to the nearest quarter inch
- **Read the trend, not the week.** Day-to-day waist swings of half an inch come from food volume, sodium and bowel timing. Three weeks of direction is signal; one week is noise. Say this out loud the first time a week goes the wrong way, because it will.
- Also worth having: **monthly progress photos** and how clothes fit, as the qualitative backup.
- **Guardrail (second signal):** lifts holding = the deficit is right. **Lifts falling across two consecutive sessions on the same movement = deficit too aggressive or protein too low, and the fix is food, not less training.** With no tape and no scale, this is the early-warning system.
- Target rate: **0.5–1 lb of fat per week.** Faster than that in a 50-year-old-style recomp usually means muscle going with it.

### What this phase does NOT change
Rep ranges on the main lifts. Rest periods on the main lifts. The progression logic. He is still trying to add weight to the bar — that is the point.

---

## SCAPULA — quiet since Sep 16. Watch, do not declare victory.

**History: three episodes in fourteen weeks.** Jun 9 (65 lb DB RDL, unstrapped) · Aug 21 (hoisting a 50 lb DB to the knee, session aborted) · Sep 10 (mid-set on the Smith RDL at 165). I called it resolved on Sep 7 and it flared on Sep 10, so the bar for clearing it now is behavior over time, not a single clean session.

**Last complaint: Sep 16**, when he held the lat pulldown at 115 because it felt "a little tight." Since then, **six consecutive sessions with zero complaints**, including:
- Smith deadlifts (Sep 19) and **barbell deadlifts from the floor at 155** (Oct 9) — loaded hinge, the Sep 10 mechanism
- Hanging knee raises (Sep 14, Sep 25), 80 lb DB bench, cable rows back to 150, pulldowns back to 135 (Oct 10)

**RDL SUSPENSION LIFTED.** The three-clean-lower-sessions bar is met (Sep 19, Sep 25, Oct 9). Loaded hinging is back in. Keep it in the 8–12 rep range at moderate load; **do not run the load curve that broke it in August (205 → 235 in six days).**

### Standing rules — these do NOT expire
- **Every dumbbell comes off a rack at hip height or higher. Never hoisted from the floor to the knee.** Two of the three episodes were this exact movement.
- Thoracic mobility twice weekly, indefinitely.
- At the first sign of tightness: hold the weight, finish the session, and report it. He does this well without being told.
- **He has still not seen a physical therapist.** Recommended Aug 24 and again Sep 14. Three strains at one site means something structural is unexplained. It is quiet now, which makes this the EASY time to get it assessed rather than the urgent one. Raise it once more, then let it be his call.

## RESOLVED — lower back (was the Aug 10 active issue)

The Aug 3–8 lower back complaints stopped once the hinge was periodized down. He has run **Smith RDL at 165 total for 3×10** on Aug 29 and Sep 6 with zero back complaints, unstrapped. The earlier problem was the load curve (205 → 235 in six days), not the movement. **Keep the hinge in the 8–12 rep range at moderate load. Do not chase heavy fives on the RDL again.**

**NOTE (Sep 14): the lumbar spine remains fine — but the loaded RDL is now suspended anyway, because on Sep 10 it aggravated the SCAPULA, not the low back. Different tissue, different reason. See the active issue above.**

---

## Current working weights — HOME GYM, Costa Rica (as of Oct 13, 2026)

### Upper
| Lift | Current | Next step |
|------|---------|-----------|
| **DB Bench Press** | **80 lb** × 9/8/6 (Oct 10) | New high — was capped at 75 at PF. Hold 80, build to 3×8. He prefers the free bar/DBs over the Smith; he said so twice. |
| **DB Shoulder Press** (LEAD LIFT) | **60 lb** × 8/8/8 (Oct 10) | Third session confirming 60. Build to 3×10. Stays first. **Rack the DBs at hip height.** |
| Incline DB Bench | 75 lb × 10/9/9 (Sep 21) | Alternate with flat. Retest at the home gym where 80s exist. |
| **Seated Cable Row** | **150 lb** × 10/10 (Oct 10) | Back to pre-injury territory, pain-free. Chase 3×12 at 150. |
| **Lat Pulldown** | **135 lb** × 10/10/9 (Oct 10) | Also back to pre-injury. Go 3×10 clean, then 150. |
| Face Pulls | **70 lb** × 15 × 3 (Oct 10, home stack) | Home gym cable runs much heavier than PF's 30 lb. 70 is correct here. |
| Lateral Raise | 15 lb × 15 × 3 | Consistent for months. |
| Reverse Cable Fly | 10–15 lb/side × 12 | Light by design. |
| Skull Crusher | 40 lb bar × 12 (Sep 16, Sep 21) | **Fully cleared** and running at volume. |
| Incline DB Curl | 25 lb × 10–12 | |
| Hammer Curl | 25–30 lb × 12 | 30 lb works but fades by set 2. |
| Rope Pushdown | **90 lb** × 12, 80 on the last set (Oct 10, home stack) | Home stack. Not comparable to the 30–60 lb PF numbers. |
| HS Supine Bench (travel) | 100 lb/arm × 10/10/8 (Sep 30) | Travel baseline only. |

### Lower
| Lift | Current | Next step |
|------|---------|-----------|
| **Barbell Back Squat** (FREE) | **205 lb × 8/7/6** (Oct 12, with a rep in reserve on set 3) | Up from 6/6 three days earlier — 21 reps vs 16 at the same load. Hold 205 and close out 3×8; he left one on the table, it is right there. **SAFETY PINS BELOW DEPTH, EVERY SET — he trains alone.** |
| **Barbell Deadlift** (floor) | **155 lb** × 10, 10 (Oct 9) | Back in the program after months off. Highest-risk lift he owns. 10 lb at a time, 8–12 reps, never on a bad-sleep day. |
| Smith Squat | 205 (90/side) × 3×8 clean (Sep 14, Sep 25) | Fallback / travel option now that the free bar is in. |
| 45° Back Extension | Bodyweight 3×12–15 | Ran it Sep 14 and Sep 25 — he said it was "tougher than I thought." Keep it as the hinge on any day the deadlift is skipped. |
| **Seated Leg Curl** (home machine) | **88 lb × 3 full sets, called it "fine"** (Oct 12, on sore hamstrings) | Stall fully broken. 88 is owned. Build to 3×12, then 95–100. Ignore the PF 80 and the Sep 25 "115–125" — that unit was miscalibrated. |
| **Leg Extension** (new home machine) | **90 lb × 12** on set 3; opened at 75 × 12 × 2 (Oct 12) | He opened light because he "felt heavy" on set 1 — sore and under-recovered. 90 for 12 is confirmed. Program 90 for all 3 sets. |
| Walking Lunge (DB) | 30 lb × 12/11/10 per leg (Oct 12) | One good set off a clean 3×12. Hold 30 until all three land, then 35. |
| **Hip Thrust Machine** | **180 lb × 12 × 2** (Oct 12; opened at 140, easy) | Retest done. 180 confirmed with room to spare. **Go 200 next Day A.** Runs every other lower session per his request. |
| Glute Lift Machine (travel) | 100 lb × 12 (Sep 14) | Travel substitute. |
| Leg Press / Squat Machine | Available at home, unused since July | Variety rotation only — free barbell squat is the primary. |

### Core (rotate, never repeat a circuit back to back)
Pallof Press 22.5 lb × 12/side · KB Plank Drag **30 lb** × 20 (20 felt light) · Dead Bugs 20–24 · Side Plank 45 sec/side · Plank Shoulder Tap 20 · Hanging or machine Knee Raise 10–12 · Bird Dog 16

### Rest periods — he standardized these himself and flagged them for data
2 min on main compounds, 90 sec on accessories, 45 sec between core rounds.

---

## ENCODING BUG — STILL LIVE. ROOT CAUSE FOUND. ONE-LINE FIX.

**I wrongly declared this fixed on Sep 14.** I verified against a stale raw.githubusercontent copy that predated Brandon's app save — the exact CDN-lag trap this file warns about. Verified again Oct 11 against the true file: **210 `Ã` and 337 `Â` sequences, re-mangled one generation from the repair.**

### Root cause — `index.html`, WorkoutLogSync
The read and the write use different encodings.

**Line 2311 — READ (wrong):**
```js
existing = JSON.parse(atob(meta.content.replace(/\n/g,'')));
```
`atob` yields raw bytes as latin-1 characters.

**WRITE (correct, UTF-8):**
```js
const b64 = btoa(unescape(encodeURIComponent(payload)));
```

Asymmetric. Every app save re-reads UTF-8 bytes as latin-1 and re-encodes them, so each non-ASCII character doubles in byte length on every cycle. `·` became tens of thousands of bytes and the file hit 1.05 MB before the Aug 24 repair.

### The fix — change line 2311 to:
```js
existing = JSON.parse(decodeURIComponent(escape(atob(meta.content.replace(/\n/g,'')))));
```
That makes the read symmetric with the write. **Until this ships, every app save re-corrupts the log and the repair has to be redone.**

### Verification rule — do not repeat my mistake
**Never verify a push against `raw.githubusercontent.com` immediately after a write.** It lags 1–5 minutes and will happily serve the pre-write copy. Verify on the blob page (`github.com/.../blob/main/<file>`) and check the "Latest commit" line, or wait and re-fetch with a cache-buster.

---

## Nutrition — THIS IS THE ACTUAL PROJECT
**Targets already on file: 1,900 kcal/day, 140 g protein. Untracked since May 17 — five months.**

**DIAGNOSED Oct 11: nothing is broken.** Both GitHub syncs share one token (`WorkoutLogSync._headers` calls `GitHubSync.getToken()`), and his workout-log pushes have been landing fine — so the token is valid and the push path works. `fitness-data.json` has not updated because **he simply has not pressed "Save Day" on the nutrition tab since May 17.** He kept logging workouts and stopped logging food.

**Brandon chose (Oct 11) to resume tracking in the app.** So the fix is behavioral, not technical: start pressing Save Day. One caveat in the code worth knowing — `GitHubSync.push` opens with `if(!token) return;`, which fails **silently**, while `WorkoutLogSync.push` toasts a warning. If nutrition data ever stops again with no visible error, that silent return is the first suspect.
- **Protein 140 g is the non-negotiable number** — it is what makes the deficit cost fat instead of muscle.
- **Alcohol is the first cut.** He named it himself as elevated through the travel stretch.
- Expect the first 2–3 weeks to show faster visible change than the real fat loss rate, because travel bloat, water and inflammation clear first. Do not let him over-read that, or under-read the slowdown after.

### Measurement — NO SCALE, but WEEKLY WAIST TAPE (his choice, Oct 11)
- **NO SCALE — he does not want to weigh himself. Do not ask for weight, do not ask him to reconsider.**
- **Waist at the navel, once a week.** He offered this himself after initially declining. It is the primary number and it is literally the thing he is trying to change.
- **Protocol matters more than the number** — an inconsistent measurement is worse than none:
  - Same morning each week, before eating or drinking
  - Level with the navel, tape parallel to the floor all the way around
  - **At the end of a normal exhale. Not sucked in, not pushed out.**
  - Snug against skin without compressing it
  - Record to the nearest quarter inch
- **Read the trend, not the week.** Day-to-day waist swings of half an inch come from food volume, sodium and bowel timing. Three weeks of direction is signal; one week is noise. Say this out loud the first time a week goes the wrong way, because it will.
- Also worth having: **monthly progress photos** and how clothes fit, as the qualitative backup.
- **Guardrail (second signal):** lifts holding = the deficit is right. **Lifts falling across two consecutive sessions on the same movement = deficit too aggressive or protein too low, and the fix is food, not less training.** With no tape and no scale, this is the early-warning system.
- Target rate: **0.5–1 lb of fat per week.** Faster than that in a 50-year-old-style recomp usually means muscle going with it.

### What this phase does NOT change
Rep ranges on the main lifts. Rest periods on the main lifts. The progression logic. He is still trying to add weight to the bar — that is the point.

---

## SCAPULA — quiet since Sep 16. Watch, do not declare victory.

**History: three episodes in fourteen weeks.** Jun 9 (65 lb DB RDL, unstrapped) · Aug 21 (hoisting a 50 lb DB to the knee, session aborted) · Sep 10 (mid-set on the Smith RDL at 165). I called it resolved on Sep 7 and it flared on Sep 10, so the bar for clearing it now is behavior over time, not a single clean session.

**Last complaint: Sep 16**, when he held the lat pulldown at 115 because it felt "a little tight." Since then, **six consecutive sessions with zero complaints**, including:
- Smith deadlifts (Sep 19) and **barbell deadlifts from the floor at 155** (Oct 9) — loaded hinge, the Sep 10 mechanism
- Hanging knee raises (Sep 14, Sep 25), 80 lb DB bench, cable rows back to 150, pulldowns back to 135 (Oct 10)

**RDL SUSPENSION LIFTED.** The three-clean-lower-sessions bar is met (Sep 19, Sep 25, Oct 9). Loaded hinging is back in. Keep it in the 8–12 rep range at moderate load; **do not run the load curve that broke it in August (205 → 235 in six days).**

### Standing rules — these do NOT expire
- **Every dumbbell comes off a rack at hip height or higher. Never hoisted from the floor to the knee.** Two of the three episodes were this exact movement.
- Thoracic mobility twice weekly, indefinitely.
- At the first sign of tightness: hold the weight, finish the session, and report it. He does this well without being told.
- **He has still not seen a physical therapist.** Recommended Aug 24 and again Sep 14. Three strains at one site means something structural is unexplained. It is quiet now, which makes this the EASY time to get it assessed rather than the urgent one. Raise it once more, then let it be his call.

## RESOLVED — lower back (was the Aug 10 active issue)

The Aug 3–8 lower back complaints stopped once the hinge was periodized down. He has run **Smith RDL at 165 total for 3×10** on Aug 29 and Sep 6 with zero back complaints, unstrapped. The earlier problem was the load curve (205 → 235 in six days), not the movement. **Keep the hinge in the 8–12 rep range at moderate load. Do not chase heavy fives on the RDL again.**

**NOTE (Sep 14): the lumbar spine remains fine — but the loaded RDL is now suspended anyway, because on Sep 10 it aggravated the SCAPULA, not the low back. Different tissue, different reason. See the active issue above.**

---

## Current working weights — HOME GYM, Costa Rica (as of Oct 13, 2026)

### Upper
| Lift | Current | Next step |
|------|---------|-----------|
| **DB Bench Press** | **80 lb** × 9/8/6 (Oct 10) | New high — was capped at 75 at PF. Hold 80, build to 3×8. He prefers the free bar/DBs over the Smith; he said so twice. |
| **DB Shoulder Press** (LEAD LIFT) | **60 lb** × 8/8/8 (Oct 10) | Third session confirming 60. Build to 3×10. Stays first. **Rack the DBs at hip height.** |
| Incline DB Bench | 75 lb × 10/9/9 (Sep 21) | Alternate with flat. Retest at the home gym where 80s exist. |
| **Seated Cable Row** | **150 lb** × 10/10 (Oct 10) | Back to pre-injury territory, pain-free. Chase 3×12 at 150. |
| **Lat Pulldown** | **135 lb** × 10/10/9 (Oct 10) | Also back to pre-injury. Go 3×10 clean, then 150. |
| Face Pulls | **70 lb** × 15 × 3 (Oct 10, home stack) | Home gym cable runs much heavier than PF's 30 lb. 70 is correct here. |
| Lateral Raise | 15 lb × 15 × 3 | Consistent for months. |
| Reverse Cable Fly | 10–15 lb/side × 12 | Light by design. |
| Skull Crusher | 40 lb bar × 12 (Sep 16, Sep 21) | **Fully cleared** and running at volume. |
| Incline DB Curl | 25 lb × 10–12 | |
| Hammer Curl | 25–30 lb × 12 | 30 lb works but fades by set 2. |
| Rope Pushdown | **90 lb** × 12, 80 on the last set (Oct 10, home stack) | Home stack. Not comparable to the 30–60 lb PF numbers. |
| HS Supine Bench (travel) | 100 lb/arm × 10/10/8 (Sep 30) | Travel baseline only. |

### Lower
| Lift | Current | Next step |
|------|---------|-----------|
| **Barbell Back Squat** (FREE) | **205 lb × 8/7/6** (Oct 12, with a rep in reserve on set 3) | Up from 6/6 three days earlier — 21 reps vs 16 at the same load. Hold 205 and close out 3×8; he left one on the table, it is right there. **SAFETY PINS BELOW DEPTH, EVERY SET — he trains alone.** |
| **Barbell Deadlift** (floor) | **155 lb** × 10, 10 (Oct 9) | Back in the program after months off. Highest-risk lift he owns. 10 lb at a time, 8–12 reps, never on a bad-sleep day. |
| Smith Squat | 205 (90/side) × 3×8 clean (Sep 14, Sep 25) | Fallback / travel option now that the free bar is in. |
| 45° Back Extension | Bodyweight 3×12–15 | Ran it Sep 14 and Sep 25 — he said it was "tougher than I thought." Keep it as the hinge on any day the deadlift is skipped. |
| **Seated Leg Curl** (home machine) | **88 lb × 3 full sets, called it "fine"** (Oct 12, on sore hamstrings) | Stall fully broken. 88 is owned. Build to 3×12, then 95–100. Ignore the PF 80 and the Sep 25 "115–125" — that unit was miscalibrated. |
| **Leg Extension** (new home machine) | **90 lb × 12** on set 3; opened at 75 × 12 × 2 (Oct 12) | He opened light because he "felt heavy" on set 1 — sore and under-recovered. 90 for 12 is confirmed. Program 90 for all 3 sets. |
| Walking Lunge (DB) | 30 lb × 12/11/10 per leg (Oct 12) | One good set off a clean 3×12. Hold 30 until all three land, then 35. |
| **Hip Thrust Machine** | **180 lb × 12 × 2** (Oct 12; opened at 140, easy) | Retest done. 180 confirmed with room to spare. **Go 200 next Day A.** Runs every other lower session per his request. |
| Glute Lift Machine (travel) | 100 lb × 12 (Sep 14) | Travel substitute. |
| Leg Press / Squat Machine | Available at home, unused since July | Variety rotation only — free barbell squat is the primary. |

### Core (rotate, never repeat a circuit back to back)
Pallof Press 22.5 lb × 12/side · KB Plank Drag **30 lb** × 20 (20 felt light) · Dead Bugs 20–24 · Side Plank 45 sec/side · Plank Shoulder Tap 20 · Hanging or machine Knee Raise 10–12 · Bird Dog 16

### Rest periods — he standardized these himself and flagged them for data
2 min on main compounds, 90 sec on accessories, 45 sec between core rounds.

---

## Encoding bug — FIXED, confirmed Sep 14

The mojibake corruption in `workout-log.json` (special characters double-encoding on every app save, ballooning the file to 1.05 MB) was repaired Aug 24. **Brandon saved a session through the app on Sep 14 and the corruption did NOT return** — zero `Ã`/`Â` sequences, file size proportionate. Keep spot-checking on each read, but the bug appears resolved.

---

## WEIGHT — 188.8 lb, Oct 12 2026. First reading in five months.

| Date | Weight | Note |
|------|--------|------|
| Apr 12, 2026 | 181.6 lb | Program start |
| May 7, 2026 | **176.8 lb** | The low. Last logged weight before the gap. |
| **Oct 12, 2026** | **188.8 lb** | **+12.0 lb vs the May low · +7.2 lb vs the April start** |

**The rate: 0.53 lb/week over 23 weeks — roughly a 266 kcal/day average surplus.** That is a modest, slow drift, not a blowout. It is consistent with mostly-reasonable eating plus a bad three-month travel stretch, all of it untracked since May 17.

### Honest composition read
**Some of it is muscle. Most of it is not.** The strength gains over those same five months are real and documented: bench 185 for 5/5/5/4 → 185 for 9/9 · DB bench 75 → 80 · shoulder press 55-was-a-struggle → 60 for 8/8/8 · Smith squat 185 → 215 and now a free bar at 225 · leg curl 70 → 88 · cable row back to 150. You do not add that without adding tissue. But a man his age does not gain 12 lb of muscle in five months while traveling and drinking more than usual. **Best estimate: 3–5 lb lean, 7–9 lb fat.** That matches his own report of noticeable belly fat.

### The useful frame — do not let him miss this
**Getting back to ~180 now would look and perform nothing like 181.6 did in April**, because of what he has built underneath. The target is not the April number, it is the April number with five months of strength on top. That makes this a recomp win in progress, not a failure to undo.

### Implications
- **This validates the fat loss phase**, which he started Oct 12 — two days before this reading. The timing is right.
- **Nutrition tracking is now the whole ballgame.** Five months dark and +12 lb is one story, not two. He committed Oct 11 to resuming Save Day in the app.
- **Realistic path: 0.5–1 lb/week.** 8 lb of fat is 8–16 weeks. Do not chase faster — faster costs the strength he just spent five months buying.
- **Counter-evidence worth citing when he gets discouraged: resting heart rate 46 bpm.** He is carrying more weight and is cardiovascularly in excellent shape. This is not a man who fell apart.

### Measurement policy — SETTLED Oct 13

**Weekly weigh-in is IN, on THURSDAY MORNINGS.** Brandon proposed Wed or Thu himself, reasoning that it puts distance between the reading and weekend drinks or a sandwich. That reasoning is correct — alcohol and high-sodium food hold water for 2–3 days — and Thursday was chosen as the later of the two, giving a full Mon–Wed washout. It also sits 3 days clear of Monday's heavy lower session, so squat-related inflammation and glycogen water have settled.

**Weight and waist get measured the SAME Thursday morning, same conditions.** One weekly ritual, not two:
- After the bathroom, **before eating or drinking anything**
- Minimal clothing, same amount each week
- Waist level with the navel, tape parallel to the floor, **at the end of a normal exhale** — not sucked in
- Weight to the nearest 0.2 lb, waist to the nearest quarter inch

**Consistency of conditions matters more than the exact day.** A reading taken at a different time of day or after food is not comparable and is worse than no reading.

**Read the trend, not the week.** 2–4 lb of day-to-day weight noise is normal and so is half an inch on the tape. **Three weeks of direction is signal; one week is noise.** Say this out loud the first time a week goes the wrong way, because it will — and he has a history of reading single data points as verdicts (see "bloated and fat," Sep 19).

**First controlled baseline: Thursday Oct 15, 2026.** The 188.8 on Oct 12 was uncontrolled — treat Oct 15 as the real starting point.

**The full dashboard:** weight (weekly Thu) · waist (weekly Thu) · strength log (every session, the guardrail) · RHR from Garmin (the recovery signal) · monthly photos.

---

## GARMIN WATCH — added Oct 13 2026. Read the trust rules before using any of it.

Brandon started wearing a Garmin ~Oct 11 and gave access to Garmin Connect via Chrome (he is signed in; `connect.garmin.com/app/home`, `/app/sleep`, `/app/stress`, `/app/heart-rate`, `/app/body-battery`). **Two days of data — nothing here establishes a trend yet. Revisit around Oct 25 for a first real read.**

### TRUST THESE
| Metric | Oct 13 reading | Why it is useful |
|--------|---------------|------------------|
| **Resting heart rate** | **46 bpm** (7-day avg also 46, but that is really a 2-day avg) | The single best number on the watch for him. Genuinely athletic for his age and training load. **A sustained rise of 5+ bpm over several days = under-recovery, illness, or too big a deficit.** This is now the early-warning system the fat-loss phase was missing. |
| **Sleep duration** | 8h 02m (bed 9:30 PM, wake 5:32 AM) | Consistent early schedule. Was previously self-reported 1–10 and mostly blank. |
| **Sleep stages** | Deep 52m · Light 5h 03m · REM 2h 07m | Deep is ~11% of total, on the low side (13–23% is typical). **Deep sleep is the stage alcohol destroys** — watch it against his drinking. |
| **Stress** | 30/100 · Rest 5h28, Low 40m, Med 1h55, **High 50m** (partial day) | He has twice volunteered feeling "agitated" (Sep 7) and "a little tired" (Sep 21). This makes that measurable. Watch whether high-stress days line up with sessions where he reports feeling heavy. |
| **Resting calories** | 1,123 by mid-day | Over 2+ weeks this becomes a better TDEE estimate than our 2,200–2,500 guess. He has long suspected his real TDEE is lower. |

### DO NOT TRUST — and do not let these into the deficit math
| Metric | Oct 13 reading | Why it is wrong |
|--------|---------------|------------------|
| **Calories burned, lifting** | **130 kcal** for a full lower-body session | Off by 3–4x. His sessions run 350–500. **Never use Garmin burn figures for lifting.** Overcounting burn is the classic way a fat-loss phase stalls. |
| **"Work time" / set count** | 10:21 work time, 14 sets, for a ~70 min session | He did not hit the set button cleanly, and it would be unreliable even if he had. |
| **Peak HR during lifting** | 109 bpm | Wrist optical HR is poor during resistance training — grip and forearm flexion corrupt the signal, and HR tracks strength effort badly anyway. |

### Standing advice given Oct 13
**Stop trying to log sets on the watch.** His own app already captures real weights, reps and notes, and does it far better. Use the watch to record the session as an activity only for HR/stress context, or do not record it at all. Duplicating his log on the watch is worse at the job.

### DEVICE: Garmin Forerunner 645 Music — confirmed Oct 13 from a photo of the case back
Released early 2018. **Roughly eight years old**, with a correspondingly old optical sensor several generations behind current Garmin hardware. This materially changes what the data is worth.

**CORRECTION — Body Battery does not exist on this watch.** On Oct 13 I told Brandon it was empty because it needed more nights of sleep data and to check back in a week. That was wrong: **the FR645 Music does not support Body Battery at all.** It will never populate. Do not tell him to wait for it.

**Also absent: Pulse Ox / SpO2.** No blood-oxygen sensor, which means no respiration-informed sleep analysis. Newer Garmins blend SpO2 and respiration into sleep staging; this one cannot, so its deep/light/REM split is built from **accelerometer plus heart rate only**. Downgrade sleep stages from "directionally useful" to **"basically noise on this hardware."** Total sleep duration remains usable. Stop quoting him deep-sleep minutes as if they mean something.

**Still solid on this device:** resting heart rate (resting PPG is the easy case and even an old sensor handles it — the 46 bpm stands), steps, and total sleep duration with the usual overestimate bias.

**Fit matters more on old hardware.** The photographed watch is visibly well worn. Worth one reminder: clean the sensor window, wear it snug, a finger's width above the wrist bone. Fit is the single biggest controllable factor in optical HR quality.

**Do not push him to upgrade.** For the two things actually driving decisions here — RHR trend and sleep duration — the 645 is adequate. A newer watch would add Body Battery and Training Readiness, which would be genuinely useful given his injury history, but it is a nice-to-have, not a requirement.

### How this changes the program
The fat-loss phase had one hard objective signal (the strength log) plus a weekly waist tape. **RHR now adds a second independent recovery signal**, which matters a lot given he will not use a scale. Guardrail becomes: waist dropping + lifts holding + RHR stable = the deficit is right. **RHR climbing while the waist drops = cutting too hard.**

---

## Nutrition — currently dark, and that is the biggest gap in the program

**`fitness-data.json` has not updated since May 17, 2026.** No calories, protein, sleep, weight, or deficit data for nearly four months. All coaching since then has been training-only. Either the app stopped saving that file or the save is broken — worth diagnosing.

**Aug 25 – Sep 5 (vacation/travel), self-reported:** ate poorly, more alcohol than typical, ~7k steps/day average, light tennis on some days, one cardio session. No lifting for roughly ten days. He came back and immediately hit PRs on bench and shoulder press, so the layoff did not cost him — if anything the rest helped.

**Targets on file (unverified against reality):** 1,900 kcal/day, 140 g protein, TDEE ~2,200–2,500. Goal is body recomposition with no deadline; scale is secondary to strength and composition.

---

## HOME GYM — Costa Rica, settled as of Oct 7 (several months)

**This is the big change. Three months of training at seven-plus gyms is over.** He is back at his own gym and explicitly asked to dial in the weights here and build a proper routine. **Every number below from Oct 9–10 is a HOME GYM number and is the baseline that matters now.** Planet Fitness and hotel numbers are historical — do not program from them.

### Equipment available
- **Full free weights**, including dumbbells past 75 lb (he immediately went to 80 on bench)
- **Barbell squat rack** — he squatted free for the first time on Oct 9
- **Hip thrust machine** he specifically likes and wants back in, "maybe every other workout"
- **Leg press**, and the **squat machine** (pendulum) he used before leaving
- Leg extension is a **NEW unit** since he left — fresh baseline at 90 lb
- Leg curl is the **original machine** — 88 lb working, which is the pre-travel calibration
- Cable stack runs heavier than PF: face pulls at **70 lb**, rope pushdown at **90 lb**

### His stated preference
**Free weights wherever possible** — his reasoning is that they are more available in crowded gyms and the skill carries when he travels. Honor that: barbell and dumbbell first, machines for the accessory and glute work.

### Free-weight transition status — UPDATED
- **Bench: free/DB, done.** 80 lb DBs.
- **Squat: TRANSITIONED, and he skipped the on-ramp.** The plan was 135 / 155 / 175 across three weeks; he went to 225 for 4 on day one, then 205 for 6×2. He got it — but **he trains alone, so safety pins set below depth are mandatory on every working set.** Working weight 205 for 6.
- **Floor deadlifts: BACK IN**, 155 × 10. Previously off the program. **This is the highest-risk lift he owns given three scapular strains and a lumbar history — progress it slowly, 10 lb at a time, and never on a bad-sleep day.**

### Still true about machine numbers
Cable stacks, leg curl units and Smith bars vary wildly between gyms — a 30 lb PF face pull and a 70 lb home face pull are the same effort. **Always log which gym and which machine.** The Sep 25 leg curl at 115–125 was a light machine, not a strength jump.

---

## Training schedule

**4 lifting sessions per 7 days. This is his long-standing norm — it has been 4/week for months (3/week before that). Do not describe it as a reduction or as "only" four.**

**The DAYS float; the SPACING is the rule.** He sets the specific days himself week to week (Thu/Sat one week, Mon/Wed the next) around travel and life. Do not assume a fixed weekday pattern — **ask or confirm which days before programming, and verify the real date with `date` first.**

What he holds constant: **roughly 4 days between sessions of the same body part**, alternating lower and upper. Cardio or rest on off days. Example weeks: Sun/Mon + Thu/Sat (Sep 6–12); Mon/Wed + weekend (Sep 14 on).

**Even spacing does NOT by itself justify more volume per session.** Total weekly volume is unchanged. Add a movement only when there is a specific gap in what is being trained — e.g. the hip thrust added Sep 10 because he had done no direct glute work since Aug 29.

---

## Standing process failure — PUSH BEFORE THE SESSION, NOT AFTER

**Oct 12: Brandon reported sore hamstrings the night before. I modified the plan — leg curl down to 77 for 2 rounds instead of 88 for 3 — and could not push it, because Chrome dropped off. He trained from the UNMODIFIED plan in the app and ran 88 for three sets.**

It was fine: he reported "fine" and no hamstring issue, and 88 is now confirmed. But the modification never reached him, and that is a systems failure, not a coaching one.

**Rule: a plan change is not delivered until it is verified live in the repo.** If the push cannot complete, say so in the same message as the advice and give the modified numbers in plain text in the chat, so the change reaches him even when the file does not. Do not describe a modified session as though the app has it.

---

## Open questions
- **Retest the hip thrust machine weight** on its first outing back — 200 lb is a pre-travel number.
- **Aug 15 session is still missing** from the log (a Saturday he cut short). Probably gone for good.
- **Nutrition has been dark since May 17.** Five months. `fitness-data.json` stopped updating. Biggest gap in the program by far, and now that he is settled it is the obvious thing to fix.
- **PT assessment still not booked.** Raised Aug 24 and Sep 14.
- He mentioned "feeling agitated" (Sep 7) and "a little tired" (Sep 21). Not training problems on their own; watch for a pattern.

## How Brandon works
- Wants **specific weights every time.** Never "moderate" or "as tolerated."
- **Ramp-up sets are a proven lever.** When he ramps he hits his numbers; when he skips them he opens light and reports feeling weak. Write the ramp explicitly into the warmup — he has said outright that if it is not written down, he does not do it.
- **Excellent in-session judgment.** Drops weight, slows tempo, resequences around occupied equipment, and stops sets at the right moment instead of grinding. Trust it and log what he actually did.
- **He will correct you, and he is usually right.** He caught a lower-day scheduling error and a misdiagnosed injury site in the same week. Take the correction, fix the record, and say so plainly.
- Will sometimes exceed the programmed weight on his own. Good instinct — ask him to flag when he is feeling strong so the bigger number gets written in rather than tested cold.
- **He dictates his logs with Wispr Flow, and it produces real transcription errors** — "265 lb dumbbells" meant 65, "1:40" meant 140, and "pull-ups, 12 reps each side" was actually Pallof press. **Errors substitute whole exercise names, not just numbers.** When anything is self-contradictory or out of character for his current level, flag it and ask rather than guessing — he corrects it immediately.
- **He sometimes re-pastes the same note twice.** Aug 15 and Aug 8 arrived as identical text. Never log a session you cannot distinguish from one already recorded — a phantom entry is worse than a missing one.
