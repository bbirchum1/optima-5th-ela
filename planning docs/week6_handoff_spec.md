# Week 6 Handoff Spec — Johnny Tremain Ch. 1-4

## Status

| File | Status |
|---|---|
| lesson-6-1-jt-ch1.html | ❌ Not built |
| lesson-6-2-jt-ch2.html | ✅ Complete (110KB, in week-6/) |
| lesson-6-3-jt-ch3.html | ❌ Not built |
| lesson-6-4-jt-ch4.html | ❌ Not built |
| lesson-6-fluency.html | ❌ Not built |
| lesson-6-checkin.html | ❌ Not built |

## What to tell the new chat

Paste this at the start:

---

**I'm building 5th grade ELA lessons for Optima Academy Online. I need to continue Week 6 — Johnny Tremain, Chapters 1-4.**

**Connected folders:**
- `optima-5th-ela` — main repo with SKILL.md, completed weeks 1-5, and week-6/ (has Day 2 done)
- `optima-4th-ela` — reference for writing scaffolding pattern
- `ELA OAO` — older files, not needed for this work

**What to read first:**
1. `optima-5th-ela/5th-grade-ela-lesson/SKILL.md` — the full rules document (1333 lines). Read Steps 0-4 for structure, Step 14 for writing, the novel identity for Johnny Tremain (~line 1092), and Steps 17-18 for fluency/check-in.
2. `optima-5th-ela/planning docs/5th_grade_ela_scope_sequence.xlsx` — Week 6 row for all scope details
3. `optima-5th-ela/week-6/lesson-6-2-jt-ch2.html` — the completed Day 2 file. Use this as the structural reference for Days 1, 3, 4.
4. `optima-5th-ela/planning docs/week6_handoff_spec.md` — this file (full specs for all remaining days)

**Novel text:** The full Johnny Tremain PDF is at `optima-5th-ela/planning docs/Johnny tremain novel copy/Johnny Tremain - Esther Hoskins Forbes.pdf`. Use `pdftotext` to extract it — it's a real text PDF, not scanned. Chapter boundaries: Ch 1 line 179, Ch 2 line 887, Ch 3 line 1413, Ch 4 line 2046, Ch 5 line 2669.

**Build approach:** Copy lesson-6-2 as a structural template. Use a Python string replacement script via bash to swap week/day/chapter numbers, then use agents or direct edits to replace all content sections. Files are ~100-110KB so they're too large for a single Write call — use bash to write them.

**CRITICAL — Writer's Workshop:** Every lesson's Writing Connection (Tab 4) must include DIRECT INSTRUCTION with scaffolding, not just a prompt. The pattern (adapted from 4th grade):
1. Progress chips showing the 6-step arc
2. 🎯 Focus callout
3. 👀 "Watch How — Alex" model writer section (green bg) with before/after or worked example
4. 📋 "Today's Tool" (blue bg) with filled example + blank student template
5. 🪶 "Sentence Frames You Can Borrow" (purple bg)
6. 📝 "Now you try" callout + graded textarea

**Please build: Days 1, 3, 4, fluency, and check-in. Day 2 is done.**

---

## Week 6 Scope (from spreadsheet)

- **Novel:** Johnny Tremain, Ch. 1-4 (D1=Ch1, D2=Ch2, D3=Ch3, D4=Ch4)
- **Grammar:** Nouns, appositives, and commas for explanation
- **Spelling:** Latin roots and affixes in academic vocabulary
- **Morphology:** Roots dict/scrib/script (say, write)
- **Reading focus:** Analyze how setting, events, and conflict change a character's path
- **Writing focus:** Argument/opinion writing — introduce claim, reasons, evidence, reasoning
- **Standards:** ELA.5.R.1.1; ELA.5.C.1.3; ELA.5.V.1.2; ELA.5.R.3.2; ELA.5.C.3.1

## Novel Identity

- Accent: Revolutionary red `#8B2500` + parchment gold `#D4A843`
- Gradient: `linear-gradient(135deg, #8B2500, #A83820)`
- Emoji: ⚒️ 🔔 📜 🐎 🗽 🔥
- Token: ⚒️
- Open Book cover: `linear-gradient(145deg, #6B1A00, #8B2500, #A83820)` spine `#4A1200`
- Open Book deco: 🔔
- Tracker path stroke: `#8B6914`

## Daily Rotation Reference

| Element | Day 1 | Day 2 | Day 3 | Day 4 |
|---|---|---|---|---|
| Arc verb | Define | Identify | Use/Apply | Explain/Justify |
| SWYK | Morphology | Grammar | Spelling | Vocabulary |
| Poetry Corner | No | Yes | No | Yes |
| RWM | No | Yes | Yes | No |
| WGRD placement | Tab 1 | Tab 1 | Tab 3 | Tab 3 |

## Writer's Workshop Arc (Weeks 6-8)

| Day | Workshop Title | What Students Learn | Progress Chip Active |
|---|---|---|---|
| 6.1 | What Is a Claim? | Claim vs. summary; write a claim about Johnny | ★ What Is a Claim? |
| 6.2 ✅ | What Are Reasons? | "Because" test; write 2 reasons | ★ Reasons |
| 6.3 | What Is Evidence? | Proof test (from text, connects, specific); find evidence | ★ Evidence |
| 6.4 | Putting It Together | Argument map: claim + reasons + evidence combined | ★ Putting It Together |
| 7.1 | Draft: Opening | Write a claim statement paragraph | ★ Draft |
| 7.2 | Draft: Body 1 | Write first reason + evidence paragraph | ★ Draft |
| 7.3 | Draft: Body 2 | Write second reason + evidence paragraph | ★ Draft |
| 7.4 | Draft: Conclusion | Write conclusion + connect to theme | ★ Draft |
| 8.1 | Revise for Meaning | ARMS (Add/Remove/Move/Substitute) | ★ Revise |
| 8.2 | Revise for Evidence | Strengthen evidence and reasoning | ★ Revise |
| 8.3 | Edit for Conventions | CUPS (Capitals/Usage/Punctuation/Spelling) | ★ Edit |
| 8.4 | Publish | Final polished argument essay | ★ Publish |

## Day-by-Day Specs (remaining days)

### Day 1 — Chapter 1: "Up and About"

**Chapter summary:** Boston 1773. Johnny is a proud, talented 14-year-old silversmith apprentice in Mr. Lapham's shop. He bosses Dove and Dusty. Mrs. Lapham runs household with daughters Madge, Dorcas, Cilla, Isannah. Johnny's secret: his dead mother said he's related to merchant Jonathan Lyte and gave him a silver cup with the Lyte crest (a rising eye) — only use if desperate. Cilla is the only one who knows.

**DOL:**
- Model: "Johnny Tremain, the most skilled apprentice in the shop, handled the silver with steady hands."
- Fix-it: "the boy a talented silversmith worked in mr laphams shop on hancocks wharf in boston"

**Quote strip:** "On Rocky Islands gulls woke. Time to be about their business."

**WGRD:** "Good readers pay attention to how a story introduces its main character. As you read today, ask yourself: What does Johnny value most? How does his talent shape the way he treats others? What hints does the author give about how this pride might cause problems?"

**Vocabulary (Decode & Discover):** apprentice, crucible, journeyman, engraver, annealing

**Morphology SWYK (graded):** "The root 'dict' means 'to say or speak.' Use this root to explain what 'predict' means. How does the root help you figure out the meaning?"

**Comprehension:**
1. "How does the author show that Johnny is different from the other apprentices? Use at least one detail."
2. "Why does Mrs. Lapham want Johnny to continue working hard even though Mr. Lapham is slowing down?"
3. "Why does Johnny keep his connection to the Lyte family a secret? What does this tell you about his situation?"

**Pause & Think:**
1. "How does Johnny feel about his own skill? How do the other boys feel about him?"
2. "Why might Johnny's mother have told him to keep the Lyte connection secret?"

**Writer's Workshop — What Is a Claim?**
- Alex model: OBSERVATION → CLAIM transformation
- Tool: Claim vs. Summary (side-by-side comparison)
- Frames: "In Chapter 1, [character] shows that ___." / "[Character]'s biggest strength/weakness is ___ because ___."

**Hero Banner:** Silversmith's workshop — workbench, tools, glowing crucible, shelves of silver, morning light, Johnny's silhouette. Warm reds/golds. Animated crucible glow.

---

### Day 3 — Chapter 3: "An Earth of Brass"

**Chapter summary:** Weeks pass. Johnny's burned hand healed but useless — thumb fused to palm. Can't work as silversmith. Wanders Boston looking for work, too proud for menial jobs. Rejected everywhere. Dove and Dusty mock him. Desperate and lonely. Finally remembers mother's words about the Lyte connection and the silver cup. Decides: tomorrow he'll go to Merchant Lyte.

**DOL:**
- Model: "The silversmith's hand, a twisted reminder of that terrible Sunday, could no longer hold a tool."
- Fix-it: "johnny once the best apprentice in boston now wandered the streets looking for any work he could find"

**Quote strip:** "He sat a long time with his arms hugging his knees. Now he knew what to do."

**WGRD (Tab 3):** "Good readers notice how a character responds to failure. Today, pay attention to how Johnny handles losing everything he was good at. Ask yourself: Is Johnny changing? What does he try? What does he refuse to do, and why?"

**Vocabulary (cloze/Day 3):** cobbler, wharf, charity, livelihood, desperate

**Spelling SWYK (graded):** "Choose one word with the root 'scrib' or 'script.' Write a sentence using that word, then explain how the root helps you understand its meaning."

**Comprehension:**
1. "How has Johnny's life changed since the accident? Describe at least two specific ways."
2. "Why does Johnny refuse some types of work even though he's desperate? What does this reveal about his character?"
3. "What finally pushes Johnny to decide to visit Merchant Lyte? Why is this a turning point?"

**Pause & Think:**
1. "Johnny just got turned away from another shop. How is he feeling? What details tell you?"
2. "Why is going to Merchant Lyte such a big decision? What is he risking?"

**Writer's Workshop — What Is Evidence?**
- Alex model: Reason → Evidence with a specific text detail
- Tool: The Proof Test (3 checks: from text, connects to reason, specific)
- Frames: "In Chapter ___, the author shows this when ___." / "The text says '___,' and this supports my reason because ___."

**Hero Banner:** Johnny alone on cobblestone Boston streets — narrow alleys, brick buildings, ship masts distant. Somber. Bandaged hand visible. Animated wind, distant ship flags.

---

### Day 4 — Chapter 4: "The Rising Eye"

**Chapter summary:** Johnny goes to Merchant Lyte's mansion with his silver cup. Lyte is wealthy, cold. Johnny presents the cup, claims he's a relative. Lyte accuses him of STEALING it — says it's from a burgled set. Johnny arrested and jailed. At trial, Rab (new character — printer's apprentice at the Boston Observer) helps him. Cilla and Isannah testify Johnny had the cup before the alleged theft. Johnny acquitted but Lyte keeps the cup. After trial, Cilla kisses Johnny's burned hand. He's moved to tears.

**DOL:**
- Model: "Merchant Lyte, a man of great wealth and influence, stared coldly at the boy standing before him."
- Fix-it: "rab a quiet apprentice at the boston observer helped johnny prove his innocence at the trial"

**Quote strip:** "She bent and kissed his burned hand. He said nothing. He was suddenly afraid he might cry."

**Poetry Corner:** "If" by Kipling (stanzas 1-2). Socratic: "Which line from the poem best describes what Johnny went through this week? Why?"

**WGRD (Tab 3):** "Good readers reflect on how a character's path has changed. Today, ask yourself: How is Johnny at the end of Chapter 4 different from Chapter 1? What has he lost? What — or who — has he gained?"

**Vocabulary (Choice Board/Day 4):** All week's words + Ch. 4: merchant, acquitted, testimony, innocence. SWYK textbox (graded).

**Comprehension (include one cross-week question):**
1. "Why does Merchant Lyte accuse Johnny of stealing instead of accepting him? What might Lyte's real motivation be?"
2. "How does Rab help Johnny during the trial? What does Rab's behavior tell you about his character?"
3. (Cross-week) "Think about Johnny from Chapter 1 to end of Chapter 4. How has his understanding of himself changed? Use details from at least two chapters."

**Pause & Think:**
1. "How did Lyte react to the cup? Were you expecting that?"
2. "Why is Cilla and Isannah's testimony so important? What would have happened without it?"

**Writer's Workshop — Putting It Together**
- Alex model: Full argument map — Claim + Reason 1 + Evidence 1 + Reason 2 + Evidence 2
- Tool: The Argument Map (2-column grid: reasons on left, evidence on right)
- Frames: "I believe that ___ because ___. For example, in Chapter ___, ___." / "Another reason is ___. The text shows this when ___."

**Hero Banner:** Colonial courtroom or Lyte's mansion — dark wood, tall windows, silver cup on table as evidence, Johnny standing small before powerful figures. Candle flicker, dust motes.

---

### Fluency

- Separate file: lesson-6-fluency.html
- Pick a strong passage from Ch. 1-4 (~150-200 words) for oral reading practice
- Suggested: the opening of Ch. 1 ("On Rocky Islands gulls woke...") or the accident scene from Ch. 2
- Follow the fluency template from previous weeks (see lesson-5-fluency.html)

### Check-In

- Separate file: lesson-6-checkin.html
- 14 points across 5 sections: grammar (appositives), morphology (dict/scrib/script), spelling (Latin roots), reading comprehension (Ch. 1-4), writing (claim/evidence)
- Follow the check-in template from previous weeks (see lesson-5-checkin.html)

## Memory notes for the new chat

- **DOL rule:** Model sentence and fix-it sentence must be TWO DIFFERENT sentences, not corrected/broken versions of the same one.
- **No copywork** anywhere in the year.
- **5 graded textboxes per lesson:** 3 comprehension + 1 SWYK + 1 Writing Connection
- **Writer's Workshop must have direct instruction** — model writer, before/after, tool template, sentence frames, then student practice. NOT just a prompt.
- Output goes to the `optima-5th-ela` folder (not ELA OAO).
