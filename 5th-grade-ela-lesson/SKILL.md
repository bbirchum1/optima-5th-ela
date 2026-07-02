---
name: 5th-grade-ela-lesson
description: >
  Build a full week of 5th grade ELA lesson HTML pages (4 separate files) for Optima Academy
  Online / Canvas LMS. Use for ANY task involving 5th grade Optima ELA — creating a new week
  of lessons, editing an existing lesson, updating strands (reading, grammar, spelling,
  morphology, vocabulary, poetry, writing), or adapting the weekly arc.
  Trigger on: "build week 3 ELA," "make the Bowditch lessons," "create lesson 9.1,"
  "build the grammar section," "generate an ELA week," or any request involving 5th grade
  ELA Canvas lesson pages for Optima Academy. Always use this skill before writing or editing
  any 5th grade ELA HTML — it contains the structure, strand rules, weekly arc, and writing
  standards.
---

# 5th Grade ELA Lesson Builder — Optima Academy Online

You are building a set of self-contained HTML lesson files for 5th grade ELA students. Each week produces **4 separate HTML files** (Lesson _.1 through _.4), each embedded in Canvas as an iframe. Students work through them independently — no live teacher required. The lessons must feel like guided, step-by-step instruction from a warm, knowledgeable teacher, not a worksheet or homework packet.

---

## Step 0 — Curriculum References

Before building any lesson, consult these reference documents:

### 5th Grade Scope & Sequence (`5th_grade_ela_scope_sequence.xlsx`)

This spreadsheet contains:
- **5th Grade Scope** tab — 32-week plan with columns for: Week, Core Reading / Chapter Pace, Reading Skill / What Good Readers Do, RWM Focus, Morphology / Vocabulary, Spelling / Word Analysis, Grammar / Conventions, Writing Focus / Assessment, and Primary 5th Grade Standards.
- **Overview** tab — Year format, core texts, and design notes for morphology, spelling, and grammar.
- **5th Grade Standards** tab — Florida B.E.S.T. ELA standards organized by strand.
- **Morphology Progression** tab — 7-phase morphology arc from bridge/review (Weeks 1–5) through cumulative transfer toward middle school (Weeks 31–32).

**Always look up the current week in the scope before writing any lesson content.** The scope tells you:
- Which chapters to assign per day
- Which grammar skill to teach
- Which spelling/word analysis rule to focus on
- Which morphology root or affix to introduce
- Which reading skill and RWM focus to use
- Which writing type and task are in play
- Which standards are primary for that week

### Florida B.E.S.T. ELA Standards — 5th Grade

**How to use the standards in lessons:**
- The objectives card on the Warm-Up tab should align with the week's primary standards, even though standard codes are NOT shown to students.
- Comprehension questions should exercise the reading standards for the week (e.g., ELA.5.R.1.1 = setting, events, conflict, characterization, plot; ELA.5.R.1.2 = theme development; ELA.5.R.1.3 = character perspective).
- Grammar tasks should align with ELA.5.C.3.1 and the specific grammar skill from the scope.
- Morphology and vocabulary tasks should align with ELA.5.V.1.2 (Greek/Latin roots and affixes, including affixes and parts of speech) and ELA.5.V.1.3 (context clues, figurative language, word relationships).

#### Standards Reference

| Strand | Standards |
|---|---|
| **Reading Literature** | ELA.5.R.1.1 analyze setting, events, conflict, characterization and plot; ELA.5.R.1.2 theme development; ELA.5.R.1.3 character perspective; ELA.5.R.1.4 poetry; ELA.5.R.3.1 figurative language; ELA.5.R.3.2 summarizing plot/theme |
| **Informational Reading** | ELA.5.R.2.1 text structures/features and meaning; ELA.5.R.2.2 central ideas and relevant details; ELA.5.R.2.3 author purpose/perspective; ELA.5.R.2.4 argument, claim, evidence, reasoning; ELA.5.R.3.3 primary/secondary source comparison |
| **Writing** | ELA.5.C.1.2 narrative; ELA.5.C.1.3 claim/argument with logical reasons, relevant evidence, elaboration, structure, varied transitions; ELA.5.C.1.4 expository using multiple sources; ELA.5.C.1.5 planning, revising, editing |
| **Foundational Skills / Fluency** | ELA.5.F.1.3 grade-appropriate phonics, word analysis, syllabication, morphology in and out of context; ELA.5.F.1.4 fluency with accuracy, automaticity, and prosody |
| **Vocabulary / Morphology** | ELA.5.V.1.1 academic vocabulary; ELA.5.V.1.2 Greek/Latin roots and affixes, including affixes and parts of speech; ELA.5.V.1.3 context clues, figurative language, word relationships, reference materials, background knowledge |
| **Grammar / Conventions** | ELA.5.C.3.1 grammar, punctuation, capitalization, and spelling appropriate to grade level |
| **Speaking, Research, Digital** | ELA.5.C.2.1 oral presentation with pacing; ELA.5.C.4.1 research using multiple reliable/valid sources; ELA.5.C.5.1 multimedia for emphasis; ELA.5.C.5.2 digital writing tools |

### Core Texts (in order)
1. *The Witch of Blackbird Pond* by Elizabeth George Speare (Weeks 1–5)
2. *Johnny Tremain* by Esther Forbes (Weeks 6–8)
3. *Carry On, Mr. Bowditch* by Jean Lee Latham (Weeks 9–14)
4. *Soft Rain* by Cornelia Cornelissen (Weeks 15–18)
5. *How I Became a Ghost* by Tim Tingle (Weeks 19–25)
6. *By the Great Horn Spoon!* by Sid Fleischman (Weeks 26–30)
7. Year-end synthesis and presentations (Weeks 31–32)

### Required Materials (shown on every lesson's "You'll need" strip)
- 📓 Reading Journal
- ✏️ Pencil
- 📕 Your Novel

Do NOT list headphones, highlighters, or other optional items.

### HTML Template Reference (`template-lesson.html`)

This file is the **canonical template** for all 5th grade ELA lessons. It lives in the same folder as this skill file. **Always read the template before building a lesson.** It contains:

- The complete CSS design system (all component styles, colors, interactive game styles, journal textbox styles, open book card, tracker, etc.)
- The 4-tab HTML structure: Warm-Up → Word Study → Reading → Assignment
- All interactive JS: word sort, vocab match, fill-in-the-blank, DOL self-check, flip cards, gathered answers, copy-to-clipboard, download-as-PDF, confetti, progress bar, tab switching, back-to-top, story journey tracker, collapsible intro
- The "Learn & Practice" / "Show What You Know" two-part structure within each Word Study section
- The open book card with layered cover, spine, page layers, and left/right page layout
- The gathered answers review box on the Assignment tab with per-question textboxes
- The narrative transition bridges between tabs

**When building a new lesson:**
1. Read this SKILL.md for rules and content decisions.
2. Read the template HTML for the exact structure, CSS classes, and JS functions to use.
3. Look up the week in the Scope & Sequence for content (chapters, grammar, spelling, morphology, etc.).
4. Look up the novel in the Novel Identity System for colors, emoji, and cover styles.
5. **Wait for the user to provide chapter text or notes** before writing any content that references specific plot points, quotes, character actions, or chapter events. (See "Novel Content Accuracy" below.)
6. Duplicate the template and replace all content placeholders with the week's actual content.

**Do NOT redesign the template.** Use the same CSS, JS, and HTML structure. Only the content inside the components changes — the components themselves stay the same.

### Novel Content Accuracy

**CRITICAL: Never guess at novel content.** Quotes, plot points, chapter events, character actions, DOL sentences, poetry connections, grammar game sentences, RWM sentences, comprehension questions, and Pause & Think prompts all depend on what actually happens in the text. Getting these wrong undermines the entire lesson.

**The rule:** Before building any lesson, the user will upload the chapter text, their notes, or a summary of the relevant chapters. All novel-specific content must be pulled from what the user provides — not from memory or general knowledge.

**What requires uploaded source material:**
- Comprehension questions (must reference actual events, not assumed ones)
- DOL sentences (must use actual character names, places, and events from the chapters)
- Grammar examples (must use sentences from or closely inspired by the chapters)
- Grammar game sentences (must feel like they belong in the novel)
- Pause & Think prompts (must reference actual chapter events)
- RWM sentences (must be pulled directly from the text)
- Fluency passages (must be an actual excerpt)
- Quote strip (must be an actual quote from the novel)
- Vocabulary words (must actually appear in or connect to the chapters)
- What Good Readers Do framing (must connect to what actually happens in the chapters)

**What can be built without source material:**
- The HTML template structure, CSS, and JS (these never change)
- Grammar rules and spelling rules (these come from the scope, not the novel)
- Morphology root/affix lessons (these come from the scope)
- Interactive game mechanics (sort, match, fill-in-blank — the structure is the same regardless of content)
- Tab transitions, objectives format, video placeholders, need strip, info strip

**If the user asks you to build a lesson without providing chapter text:** Ask for it. Say something like: *"I can set up the full lesson structure with the grammar, spelling, and morphology content from the scope. But to write accurate comprehension questions, DOL sentences, and Pause & Think prompts, I'll need the chapter text or your notes for [chapters X–Y]. Can you upload those?"*

---

## File Naming Convention

```
lesson-[week]-[day]-[slug].html        (daily lesson)
lesson-[week]-fluency.html             (weekly fluency — separate file)
lesson-[week]-checkin.html             (weekly check-in — separate file)
```

Examples:
- `lesson-9-1-bowditch-ch1-2.html`
- `lesson-9-2-bowditch-ch3.html`
- `lesson-9-3-bowditch-ch4.html`
- `lesson-9-4-bowditch-ch5.html`
- `lesson-9-fluency.html`
- `lesson-9-checkin.html`

A full week produces **6 files**: 4 daily lessons + 1 fluency page + 1 weekly check-in.

---

## The Two Week Types

Before building anything, identify which type of week this is. The structure is different for each.

| Week Type | When It Occurs | What Changes |
|---|---|---|
| **Skill-Building Week** | Most weeks | All strands active. Normal weekly arc. |
| **Pre-Project Week** | 1–2 weeks before a writing project | Normal strands Mon–Tue; writing process begins Wed–Thu. Grammar/spelling may drop. |
| **Writing Project Week** | ~Once per quarter | Writing process replaces all strands. Objectives follow writing-process arc. |

This skill covers **Skill-Building Weeks** primarily. Pre-project and project weeks use the same HTML template and design system but with adapted objectives and strand sections.

---

## Step 1 — Gather Required Information

Before building any lesson, **look up the week in the Scope & Sequence** (see Step 0). The scope tells you everything in the left column below. Confirm you have all fields before writing anything.

| Field | Where to Find It | Example |
|---|---|---|
| Week number | User request or scope | `9` |
| Novel / text | Scope: "Core Reading" column | *Carry On, Mr. Bowditch* |
| Chapter(s) per day | Scope: "Core Reading" column (D1/D2/D3/D4 breakdown) | D1 Ch. 1, D2 Ch. 2, D3 Ch. 3, D4 Ch. 4 |
| Grammar topic | Scope: "Grammar / Conventions" column | Active and passive voice awareness |
| Spelling rule | Scope: "Spelling / Word Analysis" column | Vowel teams and variant vowel patterns in domain vocabulary |
| Morphology focus | Scope: "Morphology / Vocabulary" column | Roots naut / nav: ship, sailor; port: carry |
| Reading skill | Scope: "Reading Skill / What Good Readers Do" column | Analyze characterization through obstacles, goals, and perseverance |
| RWM focus | Scope: "RWM Focus" column | Using precise academic vocabulary in expository writing |
| Writing task | Scope: "Writing Focus / Assessment" column | Expository writing: choose a research question |
| Primary standards | Scope: "Primary 5th Grade Standards" column | ELA.5.R.1.1; ELA.5.C.1.4; ELA.5.C.4.1; etc. |
| Vocabulary words | Choose 4–6 from the week's chapters | Words that connect to the morphology root or are important to the text |
| Poetry | Days 2 & 4 only — a connected poem | A poem that connects to the novel's themes |

Once you have the week's content, apply the **Define → Identify → Use → Explain/Apply** arc from Step 2 to determine how each strand's objective and task change across the 4 days.

---

## Step 2 — Understand the Weekly Arc

Every skill-building week follows a 4-day **Define → Identify → Use → Explain/Apply** arc. This arc applies to **every strand** (grammar, spelling, morphology, vocabulary). The reading objectives stay consistent across the week but the comprehension questions deepen each day.

**This arc determines the action verbs in each day's objectives AND the type of task in each section's "Show What You Know" response.** For example, if the scope says the grammar topic is "active and passive voice," the arc determines:
- Day 1: Students will *define* active and passive voice.
- Day 2: Students will *identify* active and passive voice in sentences from the novel.
- Day 3: Students will *rewrite* sentences from passive to active voice.
- Day 4: Students will *explain* when a writer might choose passive voice deliberately.

### Objective Verb Progression

| Day | Purpose | Grammar Verb | Spelling Verb | Reading Verb |
|---|---|---|---|---|
| _.1 | Learn | define | define | make connections and answer comprehension questions |
| _.2 | Notice | identify | sort / classify | make connections and answer comprehension questions |
| _.3 | Use | write using | apply / utilize | make connections and answer comprehension questions |
| _.4 | Explain | explain the importance of | utilize in a challenge | make connections and answer comprehension questions |

### Grammar Weekly Arc (Example: Active and Passive Voice)
- **_.1** — Students will *define* active and passive voice and identify the subject's role in each.
- **_.2** — Students will *identify* active and passive voice in sentences from the novel.
- **_.3** — Students will *rewrite* sentences, shifting between active and passive voice deliberately.
- **_.4** — Students will *explain* when and why a writer might choose passive voice for effect.

### Spelling Weekly Arc (Example: Vowel Teams in Domain Vocabulary)
- **_.1** — Students will *define* the vowel team patterns appearing in this week's domain vocabulary.
- **_.2** — Students will *sort* words by vowel team pattern.
- **_.3** — Students will *apply* the patterns by writing their own examples.
- **_.4** — Students will *use* the patterns to decode unfamiliar words in a challenge.

### Complete Daily Rotation Reference

This table summarizes everything that changes by day number. **Consult this before building any lesson.**

| Element | Lesson _.1 | Lesson _.2 | Lesson _.3 | Lesson _.4 |
|---|---|---|---|---|
| **Objective verb** | Define | Identify | Use / Apply | Explain / Justify |
| **Grammar task** | Define the skill | Identify in sentences | Write using the skill | Explain its purpose |
| **Spelling task** | Define the rule | Sort / classify | Write own examples | Challenge (riddles, etc.) |
| **Morphology game** | Fill-in-the-blank | Vocab-style match | Fill-in-the-blank | Vocab-style match |
| **Word Study SWYK** | Morphology | Grammar | Spelling | Vocabulary |
| **Warm-Up slot** | DOL only | DOL + Poetry Corner | DOL only | DOL + Poetry Corner |
| **What Good Readers Do** | Tab 1 (Warm-Up) | Tab 1 (Warm-Up) | Tab 3 (Reading) | Tab 3 (Reading) |
| **RWM** | Not present | Present (Tab 2) | Present (Tab 2) | Not present |
| **Weekly Fluency** | — | — | — | Separate file (not in the lesson page) |
| **Weekly Check-In** | — | — | — | Separate file (not in the lesson page) |
| **Vocabulary format** | Decode & Discover (3-step model) | Quick sort or match | Use it (cloze/sentence) | Vocabulary choice board |

**No copywork at any point in the year.** Poetry Corner appears on Days 2 and 4 all year long. Days 1 and 3 have DOL only (plus What Good Readers Do on Tab 1 for Days 1–2, Tab 3 for Days 3–4).

**Word Study SWYK rotation explained:** Each day, only ONE word study strand gets the graded "Show What You Know" textbox. The other strands are practice-only (interactive games, self-checks). This keeps the lesson focused: students practice all four strands but only write a graded response for one.

---

## Step 3 — The Strands and Hierarchy

A 5th grade skill-building week has strands that fall into two categories: **practice** and **graded**. The lesson should feel like: prepare → practice → read → submit.

### Practice Strands (interactive, self-checked)
- **What Good Readers Do** — A brief reading strategy framed for the day's text. A thinking prompt students hold in mind as they read.
- **Daily Oral Language (DOL)** — 1–2 sentences to correct in their notebook with a self-check reveal button.
- **Poetry Corner** — Days 2 & 4 only. Includes a Socratic prompt.
- **Morphology** — Video intro + examples + interactive game. Graded SWYK textbox only on its rotation day.
- **Vocabulary** — Video intro + flip cards + match game.
- **Grammar** — Video intro + novel examples + spotter game. Graded SWYK textbox only on its rotation day.
- **Spelling** — Video intro + rule card + word sort. Graded SWYK textbox only on its rotation day.
- **Pause & Think** — 1–2 thinking prompts during reading. Students pause and reflect.
- **RWM** — Sentence study routine (Days 2–3 only). See Step 16.

### Graded Responses (5 per lesson)
- **3 comprehension questions** — On the Assignment tab. Open-response, requiring evidence from the text.
- **1 Word Study SWYK** — On the Word Study tab. Rotates by day: _.1 = morphology, _.2 = grammar, _.3 = spelling, _.4 = vocabulary.
- **1 Writing Connection** — On the Assignment tab. A short sentence or imitation tied to the reading.

### Day 4 — Close the Week

Day 4 should feel like a week closer, not just another day. While it still assesses that day's chapter(s), it adds a reflective quality:

- The **comprehension questions** on Day 4 can include one question that looks across the entire week's reading (e.g., "How has Nat's relationship with Kit changed from the beginning of this week's chapters to the end?").
- The **Writing Connection** on Day 4 can be slightly more reflective (e.g., "What is one thing you understand about Kit now that you didn't at the start of the week?").
- The **vocabulary SWYK** (Day 4's rotation) uses the choice menu, which naturally encourages students to connect vocabulary to the full week's reading.
- The **What Good Readers Do** section on Day 4 (Reading tab) asks students to reflect on whether they used the week's strategy.

### Weekly Fluency — Separate File

Weekly fluency is a separate HTML page, not part of the daily lessons. See Step 17.

### Weekly Check-In — Separate File

The weekly check-in is a separate HTML page designed to later become a Canvas quiz. See Step 18B.

### How the Hierarchy Feels

| Tab | Purpose | Student experience |
|---|---|---|
| Warm-Up | **Prepare** | Watch, think, correct, reflect on poetry |
| Word Study | **Practice** | Watch videos, play games, one graded SWYK |
| Reading | **Notice** | Read, pause, think |
| Assignment | **Submit** | 3 chapter questions + 1 writing connection, review, submit |

---

## Step 4 — The Tab Structure

Each daily lesson uses **4 tabs** in this order:

```
Tab 1: 🌅 Warm-Up       (welcome video, objectives, Today's Path, What Good Readers Do [Days 1-2], DOL, Poetry Corner [Days 2 & 4 only])
Tab 2: 🔤 Word Study    (morphology, vocabulary, grammar, spelling — each with video + game; one SWYK textbox on rotating strand; RWM on Days 2–3)
Tab 3: 📖 Reading       (story journey tracker, reading video, open book card, chapter links, Pause & Think, What Good Readers Do [Days 3-4])
Tab 4: 📬 Assignment    (3 comprehension questions + 1 writing connection, gathered answers, copy/download, checklist)
```

### Why This Order

Warm up → learn words and skills → read with those tools → show what you know.

### Today's Path

The collapsible intro section includes a **Today's Path** roadmap — four pill-shaped steps with arrows showing the lesson flow:

```
🌅 Warm up with DOL & poetry → 🔤 Practice word study skills → 📖 Read Chapter X → 📬 Answer & submit
```

### What Goes in Each Tab

**Tab 1 — Warm-Up**
- Welcome video placeholder
- Today's objectives (3-line display)
- **What Good Readers Do** (Days 1 and 2 only) — thinking prompt
- DOL: 1–2 sentences to correct in notebook + self-check reveal button
- DOL feedback video placeholder
- **Poetry Corner** (Days 2 and 4 only)

**Tab 2 — Word Study**
Each section: video intro → brief lesson → interactive game. Only the rotating strand gets a SWYK textbox.
1. **Morphology** — video, root/affix lesson, fill-in-blank or match game
2. **Vocabulary** — video, flip cards, match game
3. **Grammar** — video, novel examples, spotter game
4. **Spelling** — video, rule card, word sort
5. **RWM** (Days 2–3 only) — sentence study routine

The strand whose day it is (see rotation table in Step 2) gets a **Show What You Know** card with a graded textbox.

**Tab 3 — Reading**
- **Story Journey Tracker** — ALWAYS present, first element on the tab
- Reading video placeholder
- **What Good Readers Do** (Days 3 and 4 only)
- **"Open Your Book" card** with novel cover colors and chapter names
- Chapter links: online book and read-aloud audio
- **Pause and Think** — side by side when 2 chapters; thinking prompts

**Tab 4 — Assignment**
- Clear intro: "This is the part you submit."
- **Part A: Chapter Thinking** — 3 comprehension questions with persistent prompts + sentence-starter textboxes
- **Part B: Word Study Connection** — references the SWYK already saved on the Word Study tab
- **Part C: Writing Connection** — 1 written response with persistent prompt + sentence-starter textbox
- **Gathered Answers** — auto-populated review box with all 5 graded responses + practice activity status
- **Copy to Clipboard** + **Download as PDF** buttons
- Turn-in checklist (4 items, confetti on completion)

---

## Step 5 — Video Slots and Workflow

### The 7 Standardized Slots

Every ELA lesson has exactly **7 video slots**. They follow a simple naming pattern:

```
[week]-[day]-[slot-type]
```

| Slot | Tab | What It's For |
|---|---|---|
| `welcome` | Top of Warm-Up | Teacher introduces the lesson — what's happening today, encouraging tone |
| `morphology` | Word Study, morphology section | Teacher introduces the week's root/affix with examples |
| `vocabulary` | Word Study, vocabulary section | Teacher models the vocabulary strategy (Day 1 decode; Days 2–4 varies) |
| `grammar` | Word Study, grammar section | Teacher introduces the grammar skill with examples from the novel |
| `spelling` | Word Study, spelling section | Teacher introduces the spelling pattern |
| `reading` | Top of Reading | Teacher introduces the chapters and the reading focus |
| `assignment` | Top of Assignment | Teacher explains what to submit and how |

**Example for Lesson 9.2:** `9-2-welcome`, `9-2-morphology`, `9-2-vocabulary`, `9-2-grammar`, `9-2-spelling`, `9-2-reading`, `9-2-assignment`

### Video Placeholder HTML Pattern

```html
<div class="video-wrap">
  <div class="video-wrap-header">
    <span style="font-size:20px;">🎬</span>
    <div>
      <div class="video-wrap-type">✏️ SECTION · ✏️ LABEL</div>
      <div class="video-wrap-title">✏️ Video Title</div>
    </div>
  </div>
  <div class="video-ratio">
    <div class="video-placeholder">
      <div class="video-placeholder-icon">✏️</div>
      <div class="video-placeholder-text">✏️ Brief description</div>
      <div class="video-placeholder-id"><!-- slot: ✏️ [week]-[day]-[type] --></div>
    </div>
  </div>
</div>
```

Replace every `✏️` with the appropriate content. The `<!-- slot: -->` comment is the ID system for linking real videos later — always include it.

### How Videos Get Added Later (OneDrive Workflow)

Videos are recorded separately and embedded after the lesson pages are built. The process:

1. **Record and upload** the video to OneDrive.
2. **Get the embed code** — right-click the video in OneDrive → Embed → copy the `<iframe>` snippet.
3. **Note the slot ID** — match it to one of the 7 slots above (e.g., `9-1-welcome`).
4. **Swap the placeholder** — find the `<!-- slot: 9-1-welcome -->` comment in the HTML, and replace the entire `.video-placeholder` div inside `.video-ratio` with the OneDrive iframe:

```html
<!-- BEFORE (placeholder) -->
<div class="video-ratio">
  <div class="video-placeholder">...</div>
</div>

<!-- AFTER (real video) -->
<div class="video-ratio">
  <iframe src="[OneDrive embed URL]"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:none;"
    allowfullscreen></iframe>
</div>
```

The `.video-wrap-header` bar above stays — only the inside of `.video-ratio` changes. The wrapper CSS handles 16:9 sizing automatically.

---

## Step 6 — Objectives Display

Each lesson opens with a clear, student-facing objectives card in Tab 1. Use the weekly arc verb for each strand. Format:

```
📖 Reading:    Students will [verb] + [specific task].
✏️ Grammar:    Students will [verb] + [grammar concept].
🔤 Spelling:   Students will [verb] + [spelling rule].
```

Objectives must use **action verbs that match the day's position in the arc**. See the weekly arc table above.

---

## Step 7 — Reading Comprehension Questions

These are the anchor of the Assignment tab. Follow these rules:

- **3 questions per day**, covering that day's chapter(s). Three well-crafted questions are better than five surface-level ones.
- Each question should require at least 2–3 sentences to answer properly.
- Questions must engage with the text — not recall alone. At least one question should ask students to explain, contrast, or analyze.
- Combine related ideas into stronger questions rather than splitting them. For example, instead of "What does Kit do when she arrives?" and "How do the Puritans react to Kit?" as two separate questions, combine: "How does Kit's arrival reveal differences between her background and the Puritan community?"
- Questions are open-response with individual textboxes.
- Every textbox has a **persistent prompt** above it (visible while typing) and a **sentence starter** as the placeholder.
- Questions are pulled from the user's uploaded chapter text (see Novel Content Accuracy in Step 0).

### Textbox Format for Comprehension Questions

```html
<div class="q-block"><div class="q-text"><span class="q-num">1</span>[Question text]</div></div>
<div class="textbox-prompt">[Instruction or hint that stays visible while typing]</div>
<textarea class="journal-box" id="journal-q1" data-label="Q1: [Short label]"
  placeholder="[Sentence starter...]"
  oninput="autoSave(this,'dot-q1');gatherAnswers();"></textarea>
```

### Question Depth Guide

| Question Type | Example Stem |
|---|---|
| Contrast | "Contrast how [Character A] and [Character B] respond to…" |
| Character Analysis | "What does [action/choice] reveal about [character] and how they are changing?" |
| Author's Craft | "Why does the author [choice]? What effect does this have?" |
| Evidence + Inference | "What evidence shows that [character] is struggling with [conflict]? What does this reveal about their perspective?" |
| Theme Development | "How does [event] connect to a larger idea the author is developing across the novel?" |
| Perspective | "How does the narrator's perspective shape the way this event is presented?" |

### 5th Grade Question Expectations

5th grade comprehension questions should push beyond basic recall and simple inference. Expect students to:
- Cite specific evidence and explain how it supports their answer
- Analyze how events, conflict, or characterization develop plot and theme
- Compare perspectives or explain how a character's perspective shapes their actions
- Identify and explain figurative language in context
- Connect individual events to whole-text themes

---

## Step 8 — Grammar Knowledge Check Rules

- **All grammar examples and practice sentences must come from or be inspired by the novel.** Do not use generic sentences unrelated to the reading. If the grammar skill is active/passive voice, find sentences in the novel that illustrate the concept. If the skill is relative clauses, use clauses that characters or the narrator would use.
- Always opens with a brief reminder of the week's grammar skill (1–2 sentences + 1 example from the novel).
- Day 1 task: define the skill in their own words.
- Day 2 task: identify the skill in provided sentences (from the novel or drafted in the novel's voice).
- Day 3 task: write original sentences using the skill (prompt should connect to the novel's characters or events).
- Day 4 task: explain the purpose or importance of the skill in writing (may reference how the author uses it in the novel).
- Include 4–5 items on Days 2 and 3; 1 open-response on Days 1 and 4.
- Grammar feedback video follows the task.
- Include a **Grammar Spotter** or similar interactive mini-game (see Step 19) that uses sentences from the novel.

### 5th Grade Grammar Scope

5th grade grammar is more complex than 4th grade. The scope includes:
- Complete sentences, fragments, and run-ons
- Sentence combining with compound subjects and predicates
- Dialogue punctuation and paragraphing
- Verb tense consistency in narrative writing
- Commas with introductory words and phrases
- Nouns, appositives, and commas for explanation
- Pronoun-antecedent agreement and clarity
- Compound and complex sentence review
- Active and passive voice awareness
- Verb tense and shifts in informational writing
- Subject-verb agreement with intervening phrases
- Prepositional phrases for clarity and detail
- Relative clauses and sentence expansion
- Subordinating conjunctions
- Quotation punctuation for cited evidence
- Pronoun point of view and consistency
- Verbals and verb phrases (as extension)
- Transitions that clarify time and cause/effect
- Avoiding comma splices and fused sentences
- Parallel structure in lists and comparisons
- Adjectives/adverbs for precision, not clutter
- Commas and punctuation for clarity in complex sentences
- Dialogue punctuation review
- Sentence variety for pacing
- Editing checklist: grammar, punctuation, capitalization, and spelling

---

## Step 9 — Spelling Rules

### Day 1 — Discover the Pattern

Day 1 spelling uses a **discovery approach**. Students are NOT told the rule first. Instead:

1. **Show two groups of example words** — side by side, with the target spelling pattern bolded or color-highlighted in each word. Do not label the groups with the rule yet.
2. **Ask discovery questions** — "Look at Group A. What do the bold letters have in common?" "Now look at Group B. What's different?" "Can you figure out the pattern?"
3. **Reveal the rule** — A "See the Rule" button reveals the rule after students have thought about it.
4. **Practice with a word sort** — Students sort new words using the pattern they just discovered.

This teaches students to notice patterns in language, not just memorize rules handed to them.

### Days 2–4

- Day 2 task: sort or classify a provided word list (reinforces the pattern).
- Day 3 task: write their own examples (3 for each pattern).
- Day 4 task: apply the rule in a challenge (riddles, cloze sentences, or "spot the odd one out").

### 5th Grade Spelling Scope

5th grade spelling/word analysis is more advanced, focusing on:
- Review syllable types and multisyllabic decoding routines
- Suffix spelling changes: drop e, double consonant, y to i
- Schwa and reduced vowels in unstressed syllables
- Accent and syllable stress in longer words
- Latin roots and affixes in academic vocabulary
- Commonly confused words in argument writing
- Word families and spelling patterns in claim/evidence/reasoning vocabulary
- Vowel teams and variant vowel patterns in domain vocabulary
- Syllable division in technical and academic words
- Schwa in multisyllabic academic words
- Spelling of -ous, -ious, and -eous words
- Assimilated prefixes and spelling shifts
- Multisyllabic decoding with roots and affixes
- Suffixes -ance / -ence and -ment as nouns
- Accent/stress changes in related word families
- Derivational suffix review with part-of-speech changes
- Spelling and meaning of abstract academic words
- Vowel alternations in related word families
- Hyphenated words, compounds, and syllable division
- Spelling generalizations for -ed, -ing, and suffixes in narrative writing
- Word origins and idioms
- Part-of-speech shifts in related words

---

## Step 10 — Vocabulary Practice (Daily, Rotating Format)

Every day includes vocabulary in the Word Study tab. The format rotates. The goal is **a little every day** — building a habit of noticing and decoding words, not just memorizing definitions.

### Daily Rotation Guide

| Day | Format | Description |
|---|---|---|
| _.1 | **Decode & Discover** | Teacher models the 3-step decoding process on ONE word. Students try the remaining words on their own, then confirm with flip cards. Match game follows. See "Day 1 Decode Format" below. |
| _.2 | **Quick Sort or Match** | Students sort words into categories (by part of speech, connotation, root) OR match words to definitions or example sentences. |
| _.3 | **Use It** | Students fill in 2–3 cloze sentences using the week's words, or choose one word and use it in an original sentence. |
| _.4 | **Vocabulary Choice** | Students select one activity from the Weekly Choice Menu (see below). This is the SWYK rotation day for vocabulary. |

### Day 1 Decode Format — "How to Figure Out Unfamiliar Words"

On Lesson _.1, vocabulary teaches the **decoding strategy**, not just the definitions. The section walks through one word using three steps:

**Step 1 — Read the Sentence (Context)**
Show the actual sentence from the novel where the word appears. Ask: "What clues does the sentence give you about what this word means?"

**Step 2 — Look at the Word Parts (Morphology)**
Break the word into prefix + root + suffix. Ask: "Do you recognize any parts? What might they mean together?"

**Step 3 — Confirm (Check the Definition)**
Reveal the actual definition. Ask: "Were you close? How did context and word parts help?"

After the modeled word, students see the remaining 3–5 words as flip cards. **Each flip card MUST include the actual sentence from the novel where that word appears**, displayed on the front of the card above the "what do you think it means? tap to check" prompt. This lets students practice the same 3-step context-decoding process on their own. The back of each card shows the definition plus a brief note connecting the definition back to the context clue.

The match game follows as practice.

### Weekly Vocabulary Choice Menu (Day 4)

Students choose **one** of the following:
1. ✍️ Use the word correctly in 2 original sentences.
2. 📖 Find an example of the word (or a related word) in your reading this week.
3. 🔤 Connect the word to a root, prefix, or suffix — explain the connection.
4. 🔄 Sort the week's vocabulary words by meaning, part of speech, or category — explain your groups.
5. 💬 Explain the word as if you're teaching it to a younger student.
6. 📝 Use two vocabulary words in a written response about something from the reading.

The vocabulary choice on Day 4 is the SWYK graded response for that day.

---

## Step 11 — Morphology (Word Study) Rules

**5th grade morphology focus: Greek and Latin roots, affixes, word families, and how affixes connect to parts of speech.**

5th grade assumes 3rd grade introduced common word parts and 4th grade practiced application. This year deepens into academic vocabulary, word families, and independent transfer.

### Morphology Progression

| Weeks | Role | Emphasis |
|---|---|---|
| 1–5 | Bridge from 4th grade into advanced application | Review morphemes, suffix rules, word families, and part-of-speech shifts while applying to historical fiction vocabulary and literary analysis. |
| 6–8 | Apply morphology to argument and historical fiction | Roots and affixes tied to claim, evidence, reasoning, belief, trust, and civic vocabulary while writing argument paragraphs and essays. |
| 9–14 | Deepen academic and technical vocabulary | Greek/Latin roots and suffixes for navigation, measurement, biography, and expository/research vocabulary; emphasis moves from recognition to independent transfer. |
| 15–18 | Use morphology in historical/informational reading | Analyze roots, affixes, word families, and abstract nouns while reading about removal, justice, citizenship, source comparison, and historical arguments. |
| 19–25 | Apply morphology to perspective, theme, and literary analysis | Roots and affixes connected to perspective, memory, life, feeling, voice, and abstract literary vocabulary while explaining theme and characterization. |
| 26–30 | Apply morphology to narrative craft, humor, and adventure | Word origins, suffixes, and part-of-speech shifts to strengthen narrative writing, spelling, and vocabulary in adventure fiction. |
| 31–32 | Cumulative transfer toward middle school | Independently analyze unfamiliar words using roots, affixes, context, word relationships, and reference tools across literary, informational, and research tasks. |

### Weekly Morphology Section Rules

Each week's morphology section should:
- Name the root/prefix/suffix and its language origin (Greek or Latin).
- Give the meaning of the word part.
- Show 3–4 example words containing that part.
- **Connect affixes to parts of speech** (e.g., "-tion changes a verb to a noun: navigate → navigation").
- Ask one guided task with a **journal textbox** for the response: "What do these words have in common?" or "Use the root to figure out what this unfamiliar word might mean."
- Include a **Root Match mini-game** (see Step 19): students tap a word containing the root, then tap its meaning. 4 pairs.
- Connect morphology to at least one vocabulary word from the week when possible.
- Connect morphology to the novel when possible.

**Morphology must not be a separate isolated lesson.** It should feel like it grows naturally out of the vocabulary or reading section.

**Morphology is submitted.** The journal textbox answer and mini-game completion status both appear in the Downloaded Journal Work PDF (see Step 21). Morphology also has its own line item in the Assignment tab turn-in checklist.

---

## Step 12 — Daily Oral Language (DOL) Rules

DOL uses a **model-then-fix** format. Students study a correct sentence first, then apply what they notice to fix a broken one.

### Format

**Sentence 1 — The Correct Model:**
- A real sentence from the chapter, displayed with clickable words.
- Students tap words and punctuation they notice are correct — capitals, commas, quotation marks, apostrophes, etc. Tapped words highlight green.
- **When a word is tapped, a brief explanation appears below the sentence** in language a 5th grader would understand (e.g., "This is a name, so it starts with a capital letter" — NOT "Proper noun — capitalized"). Words without a notable convention are plain text (not clickable). Only words with something worth noticing get the `.dol-highlight-word` class and an `onclick`.
- This is interactive practice, not graded.

**Sentence 2 — Fix It:**
- A structurally similar sentence WITH deliberate mistakes. Does not have to be from the book, but should use the novel's characters, settings, or events.
- The mistakes should mirror the conventions shown in the model (e.g., if the model shows quotation marks around dialogue, the broken sentence is missing them).
- Students rewrite the sentence correctly in their notebook, using the model as a guide.
- A "Check My Work" reveal button shows the corrected version with an explanation of what connects it to the model.

### DOL Sentence Rules

- **Sentence 1 must come from the novel** — pulled from the user's uploaded chapter text.
- **Sentence 2 should match the structure of Sentence 1** — same kind of punctuation, capitalization, or grammar pattern, but with errors.
- Errors should reflect the week's grammar skill when possible (e.g., comma splices during comma-splice week).
- The check reveal should explicitly connect the fix to the model: "Compare with the model: both sentences need quotation marks around the speech."
- DOL is in Tab 1. It is practice — not graded.

---

## Step 13 — Poetry Corner

Poetry Corner appears on **Days 2 and 4 only**, all year long. There is **no copywork** in 5th grade ELA.

| Day | Warm-Up Slot |
|---|---|
| Lesson _.1 | DOL only (+ What Good Readers Do on Tab 1) |
| Lesson _.2 | DOL + Poetry Corner (+ What Good Readers Do on Tab 1) |
| Lesson _.3 | DOL only (+ What Good Readers Do on Tab 3) |
| Lesson _.4 | DOL + Poetry Corner (+ What Good Readers Do on Tab 3) |

### Poetry Corner Rules (Days 2 & 4)
- One poem or excerpt per appearance. Can be the same poem across both days or different.
- Appears in the `.poem-box` component with title, author, and text.
- Includes a Socratic question as a thinking prompt.
- On Day 2: "What do you notice? What feeling or image stands out?"
- On Day 4: A deeper question — "How does the poet's word choice create this feeling?" or "What does this poem have in common with our reading?"
- Poems should connect to the novel's themes when possible.
- Poetry satisfies ELA.5.R.1.4 (poetry).

---

## Step 14 — Writing Connection Rules

- Appears in Tab 4, after the comprehension questions.
- 1–3 sentences in length.
- Always tied to the text or to the week's language skill.
- Should not be the same as the reading comprehension questions — it's a creative or craft-based task.
- 5th grade writing connections should push toward analytical and craft-based responses:
  - "Write one sentence from Kit's perspective describing her first impression of the Puritan meetinghouse. Use at least one vivid sensory detail."
  - "Revise this sentence to shift it from passive voice to active voice, keeping the same meaning."
  - "Use one of this week's vocabulary words in a sentence that shows you understand its meaning in the context of the novel."
  - "Imitate this sentence from the novel: [sentence]. Write your own version using a different subject but keeping the same structure."
  - "Write a claim statement about [character]'s most important decision in this chapter. Include one reason."

---

## Step 15 — What Good Readers Do

This is a named recurring course routine. It should feel like a brief, purposeful frame — not a long lesson. The goal is to give students a specific thinking habit to carry into their reading that day.

### Format

```
What Good Readers Do
[1–2 sentence framing statement that names the strategy.]

As you read today, pay attention to [specific thing]. Ask yourself:
• [Question 1]
• [Question 2]
• [Question 3 — optional]
```

Students do not submit a separate What Good Readers Do response. The strategy should connect directly to one or more of the day's reading comprehension questions, so the habit flows naturally into the assignment.

### Weekly Strategy Progression

Match the strategy to where students are in the novel:

| Novel Stage | Strategy Focus |
|---|---|
| Opening chapters | Preview, predict, notice setting and character introduction |
| Early-middle chapters | Infer character feelings, track problems and complications |
| Middle chapters | Notice character change, identify relationships and tension |
| Late-middle chapters | Identify theme clues, compare character perspectives |
| Final chapters | Summarize, reflect on character growth, connect to larger meaning |

### Examples by Day

**Day 1 (Tab 1):** Sets the lens before the week begins.
> Good readers pay attention to how setting shapes a character's choices. Kit has left everything she knows — a warm, sunny island — and arrived somewhere cold and unfamiliar. As you read today, ask yourself: How does the new setting affect Kit? What is she noticing? How does the place itself create conflict?

**Day 2 (Tab 1):** Reinforces the strategy — shorter, more focused.
> Good readers continue to track how setting creates tension. Today, as you read, ask yourself: Is Kit adjusting to this new world, or is the tension growing?

**Day 3 (Tab 3):** Placed before the chapter links — students are reading with more experience now.
> Good readers step back and ask: What is this story really about? Today, look for a moment that feels important — not just exciting, but meaningful. Ask yourself: What is the author showing us about belonging, freedom, or courage?

**Day 4 (Tab 3):** Reflective — students look back across the week's reading.
> Good readers reflect on what they've read. Before you answer the comprehension questions, think about the chapters you read this week. How has Kit's understanding of her situation changed? What caused that change?

---

## Step 16 — RWM: Read like a Reader, Read like a Writer, Mimic

RWM is a sentence-study routine that bridges reading, grammar, and writing. It appears in **Tab 2 (Word Study)** on **Lessons _.2 and/or _.3**. On weeks where it appears twice, the Day 2 sentence is simpler and the Day 3 sentence is more analytically demanding.

### Format

```
RWM — Read like a Reader, Read like a Writer, Mimic

Sentence from the story:
"[Exact sentence from the novel, in quotation marks.]"

📖 Read like a Reader
What is happening in this sentence? What does it show about the character, setting, or situation?
[1–2 sentence student response prompt]

✏️ Read like a Writer
How did the author build this sentence? Notice the [grammar element — verb choice, punctuation, prepositional phrases, clause structure, etc.].
[1–2 guided observation prompts]

🖊️ Mimic
Write your own sentence using the same pattern.
[Sentence frame, e.g.: "[Character] ___ and then ___." or "[Name] felt ___ because ___.]
```

### Sentence Selection Rules

- Always pull from the actual novel text for the week.
- Choose sentences that are well-crafted and illustrate something worth noticing — strong verb, interesting structure, effective punctuation, figurative language.
- The sentence should connect to the week's grammar skill when possible (e.g., if the week's grammar is relative clauses, find a sentence in the novel that uses one).
- Sentences should be 10–25 words — long enough to be interesting, short enough to analyze.

### RWM Grade 5 Expectations

- **Read like a Reader:** Students explain what the sentence means and what it shows. 1–2 sentences. Should include inference, not just restatement.
- **Read like a Writer:** Students identify the grammar or craft move. Guide them with a specific question (don't just say "What do you notice?"). Expect students to name the technique and explain its effect.
- **Mimic:** Students write one original sentence using the same pattern. A sentence frame should always be provided on Day 2. Day 3 can offer a lighter scaffold or none.

---

## Step 17 — Weekly Fluency (Separate File)

Weekly fluency is a **separate HTML file**, not part of the daily lesson pages. It requires Canvas's recording tool, which doesn't work inside an iframe-embedded lesson page.

### File Naming

```
lesson-[week]-fluency.html
```

Example: `lesson-9-fluency.html`

### One Per Week

Each week has one fluency page, assigned alongside the Day 4 lesson. It uses a short excerpt from the novel — a passage that is meaningful, expressive, and manageable in 3–5 sentences.

### Format

The fluency page is simpler than a daily lesson — no tabs, no interactive games. Just:

1. **Header** — Same as the daily lessons (Optima branding, lesson badge showing "Week 9 · Fluency")
2. **Passage** — 3–5 sentences from the week's chapters, displayed in the `.fluency-passage` styled box
3. **Fluency video** — Teacher reads the passage aloud (video placeholder)
4. **Steps** — Listen → Read for accuracy → Read for smoothness → Read for expression → Record and submit
5. **Self-check prompt** — "Did I say each word correctly? Did my reading sound smooth? Did my voice show the feeling?"
6. **Submission instructions** — "Record yourself reading the passage. Upload your recording to Canvas."

### Passage Selection Rules

- 3–5 sentences from the week's chapters.
- Choose a passage with expressive variety — dialogue, tension, or a description with feeling.
- Avoid purely expository or list-like passages.
- Include the passage text directly on the page.
- The passage must come from the user's uploaded chapter text (see Novel Content Accuracy in Step 0).

### Connection to the Daily Lessons

Fluency is **not referenced** on the daily lesson pages. It is assigned separately in Canvas alongside the Day 4 lesson. The skill should generate the fluency file when building a full week of lessons.

---

## Step 18 — Assessment Architecture

5th grade ELA uses a layered assessment system. Each layer is a separate deliverable.

### Assessment Layers

| Layer | Cadence | Purpose | Format |
|---|---|---|---|
| **Weekly Check-In** | Every instructional week | Verify transfer of weekly grammar, morphology, spelling/word analysis, reading, and writing concepts | Separate HTML file, designed to become a Canvas quiz |
| **End-of-Novel Project** | After each core novel or text unit | Show whole-text understanding through creative, oral, visual, multimedia, or performance-based work | Project artifact, presentation/recording, evidence, reflection |
| **Quarterly Writing Process** | Four times per year | Guide students through brainstorm, plan, draft, revise, edit, and publish | Draft checkpoints, revision evidence, final polished writing, reflection |
| **Portfolio / Year-End Synthesis** | Final weeks | Show growth as reader, writer, speaker, and word scholar | Curated samples, reflection, presentation, comparison, or multimedia product |

### 18A — End-of-Novel Projects

| Weeks | Text | Project | Required Evidence |
|---|---|---|---|
| 1–5 | *The Witch of Blackbird Pond* | Historical Fiction Inquiry Board: students show how setting, conflict, perspective, and resolution develop theme | Scene map; character perspective evidence; theme explanation; creative artifact |
| 6–8 | *Johnny Tremain* | Revolutionary Character Debate: students present and defend a claim about courage, responsibility, or liberty | Claim; text evidence; reasoning; counterpoint/concession |
| 9–14 | *Carry On, Mr. Bowditch* | Navigation and Perseverance Research Exhibit: students connect biography, navigation, obstacles, and theme | Research notes; technical vocabulary; theme evidence; short presentation |
| 15–18 | *Soft Rain* | Source and Perspective Portfolio: students compare literary/historical perspectives and track claim, evidence, reasoning | Primary/secondary comparison; central idea; author purpose; argument chart |
| 19–25 | *How I Became a Ghost* | Perspective and Theme Multimedia Project: students explain how narrator perspective, conflict, characterization, and figurative language develop meaning | Theme tracker; characterization evidence; figurative language explanation; reflection |
| 26–30 | *By the Great Horn Spoon!* | Adventure Arc Showcase: students create a storyboard, audio trailer, or visual pitch explaining conflict, pacing, humor, and theme | Plot arc; pacing evidence; humor/figurative language example; final narrative excerpt |
| 31–32 | Year-end | American Reader-Writer Portfolio: students compare themes, perspectives, conflicts, and their own growth across texts | Curated samples; cross-text analysis; morphology reflection; presentation |

### 18B — Weekly Check-In (Separate File)

The weekly check-in is a **separate HTML file** designed to later become a Canvas quiz. It is NOT integrated into the Day 4 lesson.

#### File Naming

```
lesson-[week]-checkin.html
```

Example: `lesson-9-checkin.html`

#### Check-In Components

| Component | What Students Show | Item Types |
|---|---|---|
| Grammar and conventions | Apply the weekly grammar/conventions concept in context | 1 correction/edit item; 1 identification item; 1 sentence application item |
| Morphology and vocabulary | Analyze roots, affixes, base words, word families, and context clues | Word-part breakdown; choose meaning from context; use one vocabulary word in a meaningful sentence |
| Spelling / word analysis | Transfer the weekly pattern into reading and writing unfamiliar words | Sort or decode 4–6 words; explain one spelling pattern; correct one misspelled word |
| Reading comprehension | Show the weekly What Good Readers Do skill with the assigned text | Short excerpt question; cite one detail; summarize, infer, track perspective, theme, central idea, or claim |
| Writing / RWM transfer | Imitate, revise, or compose using the week's sentence/writing focus | One RWM mimic sentence; one short response; one revision sentence showing the target skill |

#### Canvas Format

- 10–15 total points
- 6–8 auto-graded or short constructed-response items plus 1 short written, audio, or video submission
- Should take about 20–30 minutes
- Should feel like a weekly transfer task, not a long test

### 18C — Quarterly Writing Process Assignments

Each quarter includes one major writing product that moves through the full writing process.

#### Writing Process Stages

| Stage | Canvas Checkpoint | Expected Student Evidence |
|---|---|---|
| Brainstorm | Teacher video models idea generation and mentor-text connection | Idea list, quickwrite, topic web, character/problem list, research question list, or claim possibilities |
| Plan | Students organize before drafting | Story arc, paragraph plan, source note organizer, claim-reason-evidence chart, or comparison matrix |
| Draft | Students compose a complete first draft section by section | Draft submitted in Canvas or digital writing tool; teacher/model checklist available |
| Revise | Students improve meaning, organization, elaboration, voice, and evidence | Revision checklist plus highlighted changed section; peer/adult feedback when available |
| Edit | Students apply grammar, punctuation, capitalization, spelling, and morphology knowledge | Editing checklist; corrected conventions; attention to weekly grammar/spelling transfer |
| Publish / Present | Students create final polished work and reflect | Final product plus reflection on one improvement and one skill carried forward |

#### Quarterly Writing Map

| Quarter | Writing Product | Primary Process Emphasis | Weeks |
|---|---|---|---|
| Q1 | Historical narrative or literary response from *The Witch of Blackbird Pond* | Plan historically grounded scene or claim, draft, revise for dialogue/description or evidence, publish | Weeks 1–5 |
| Q2 | Expository/research writing connected to *Carry On, Mr. Bowditch* | Research question, reliable sources, organized notes, technical vocabulary, presentation | Weeks 9–14 |
| Q3 | Historical argument or source response connected to *Soft Rain* | Track claim/evidence/reasoning, compare sources, draft argument, revise citation/evidence | Weeks 15–18 |
| Q4 | Adventure narrative inspired by *By the Great Horn Spoon!* | Plan goal/obstacle/setting, draft rising action, revise for pacing/humor/action, publish | Weeks 26–30 |

### 18D — Weekly Check-In Map

| Weeks | Core Text | Check-In Focus | Writing Process Checkpoint |
|---|---|---|---|
| 1–5 | *The Witch of Blackbird Pond* | Historical setting/conflict, character perspective, theme, suffixes -ion/-ive/-able/-ity, sentence combining, dialogue, tense, introductory commas | Q1 historical narrative/literary response: plan, draft, revise, publish |
| 6–8 | *Johnny Tremain* | Character path, perspective over time, theme through historical events, claim/evidence/reasoning, roots dict/scrib/cred/fid, pronoun clarity, complex sentences | Argument/opinion writing: claim about courage, responsibility, or liberty |
| 9–14 | *Carry On, Mr. Bowditch* | Obstacles/goals/perseverance, summary, plot/character development, setting/conflict, figurative language, theme, technical roots | Q2 expository/research writing: question, notes, draft, revise, presentation |
| 15–18 | *Soft Rain* + historical sources | Central idea, author purpose/perspective, argument tracking, source comparison, roots migr/civ/just/mem/chron, cited evidence punctuation | Q3 historical argument or expository response with sources |
| 19–25 | *How I Became a Ghost* | Narrator perspective, setting/conflict, theme, summary, figurative language, characterization, word families, comma splices, parallel structure | Literary analysis: perspective/theme/characterization |
| 26–30 | *By the Great Horn Spoon!* | Adventure plot, pacing, humor, characterization, theme, roots aud/phon/claim/rupt/ject, suffixes -ize/-ist/-ism, dialogue and complex punctuation | Q4 adventure narrative: plan, draft, revise for humor/action, publish |
| 31–32 | Year-end synthesis | Compare authors' development of themes, perspectives, and conflicts; cumulative morphology/conventions | Portfolio/multimedia presentation or final literary project |

---

## Step 19 — Interactive Components

Each lesson includes 3–5 lightweight interactive mini-games built in vanilla JS + CSS (no external libraries). These are for guided practice — not graded. Their completion status is captured in the Downloaded Journal Work PDF (see Step 21).

### Available Interactive Types

| Type | When to Use | Mechanic |
|---|---|---|
| **Word Sort** | Spelling (Day 1–2) | Students tap a word from a bank, then tap the correct column. Correct sorts turn green and stick; wrong sorts shake red and bounce back. |
| **Vocab Match** | Vocabulary (Day 1–2) | Two-column grid: words on left, definitions on right. Students tap a word, then tap its definition. Matched pairs lock green. |
| **Root Match** | Morphology (Day 1–2) | Same mechanic as Vocab Match, but matches root-words to their meanings. Styled in purple. |
| **Grammar Spotter** (or similar grammar game) | Grammar (Day 1–2) | Sentences with clickable words. Students tap the word that is the grammar concept. Correct picks highlight green; wrong picks flash red and reset. |
| **DOL Self-Check** | DOL (every day) | Students type corrections in a textbox, then click "Check My Work" to reveal the corrected version. Not a game — but interactive. |
| **Flip Cards** | Vocabulary (Day 1) | Cards with word on front, definition on back. Tap to flip. |

### Rules for All Interactive Components

- **All sentences, words, and examples must come from or be inspired by the novel.** No generic content.
- Games should be quick (1–3 minutes) and not block lesson progress.
- Every game must have a clear success state (feedback message when complete).
- Games track their own completion in a JS variable (e.g., `window._rootMatchDone = true`) so the Download function can report it.
- Do not include interactive games that require students to write creatively (e.g., sentence builders). Writing tasks should use journal textboxes instead — students should just write.

---

## Step 20 — Graded Textboxes

Only **5 textboxes** appear in the entire lesson. Each one has two parts: a **persistent prompt** (visible while typing) and a **sentence starter** (as the placeholder).

### Where Textboxes Appear

| Tab | Section | Textbox For |
|---|---|---|
| Tab 2 (Word Study) | Rotating SWYK strand | Day 1: morphology. Day 2: grammar. Day 3: spelling. Day 4: vocabulary. |
| Tab 4 (Assignment) | Chapter Thinking Q1 | First comprehension question |
| Tab 4 (Assignment) | Chapter Thinking Q2 | Second comprehension question |
| Tab 4 (Assignment) | Chapter Thinking Q3 | Third comprehension question |
| Tab 4 (Assignment) | Writing Connection | One written sentence tied to the reading |

### Textbox HTML Pattern

```html
<div class="textbox-prompt">[Instruction that stays visible while student types]</div>
<textarea class="journal-box" id="journal-[id]"
  data-label="[Short label for PDF]"
  placeholder="[Sentence starter...]"
  oninput="autoSave(this,'dot-[id]');gatherAnswers();"></textarea>
```

### Rules

- The **persistent prompt** (`.textbox-prompt`) sits above the textbox in a teal bar and remains visible while the student types. It states the task clearly: "Use at least two details from the chapter" or "Write one sentence explaining Kit's perspective."
- The **sentence starter** (placeholder) gives students a way into the answer: "The turning point is..." or "Kit's reaction reveals..." It disappears when they start typing, but the persistent prompt above keeps them oriented.
- The `data-label` is what appears in the gathered answers and PDF. Keep it short and descriptive.
- Every textbox calls `gatherAnswers()` on input so the gathered review box stays current.
- Practice sections (DOL, What Good Readers Do, Pause & Think, poetry) use thinking prompts and interactive games instead of textboxes.

---

## Step 21 — Gathered Answers and Download

The bottom of the Assignment tab has a **gathered answers review box** that auto-populates when the student arrives on the tab and updates live as they type.

### What It Captures

1. **All 5 graded textbox answers**, organized by section with bold labels.
2. **Practice activity completion status**: ✅ or ⬜ for each interactive game (morphology fill-in, vocabulary match, grammar spotter, spelling sort).

### Two Submission Options

- **📋 Copy to Clipboard** — copies plain text that students paste directly into Canvas's text submission box. Labels are in ALL CAPS for visual distinction.
- **📄 Download as PDF** — opens a styled, print-ready page with bold section headings, bold question labels, and student answers in normal weight. Auto-triggers the browser print dialog.

### Placement

The gathered card, buttons, and checklist sit below the comprehension and writing questions on the Assignment tab. The flow is: answer questions → review gathered work → copy or download → check off the checklist → submit to Canvas.

---

## Step 22 — Narrative Flow Rules

The lesson should feel like a continuous guided experience, not a set of disconnected tabs. Follow these rules to create narrative flow:

### Tab Transitions

Every tab ends with a **narrative bridge** — a short italic sentence in the teacher's voice, followed by the "Continue to [next tab] →" button.

```html
<div class="tab-next-wrap">
  <p class="tab-transition-voice">[1 sentence that connects what the student just did to what comes next.]</p>
  <button class="tab-next-btn" onclick="switchTab('[next]')">Continue to [emoji] [Tab Name] →</button>
</div>
```

Example transitions:
- Warm-Up → Word Study: *"Now that your mind is warmed up, let's build the words you'll need before we open the book."*
- Word Study → Reading: *"Your vocabulary is ready and your pen is sharp. Time to open the book and step into the story."*
- Reading → Assignment: *"You've read, you've noticed, you've paused to think. Now let's put your understanding to work."*

### Novel Quote Strip

A warm cream banner sits between the info strip and the intro cards. It displays a single short quote from the novel in Lora italic, with an attribution line below. Changes per lesson.

### "Open Your Book" Card

On the Reading tab, before the read/listen links, place a styled open book card. The card is built in layers to look like an actual open book:

1. **Hard cover** — uses the novel's **Open Book cover** gradient from the Novel Identity System. Visible around all edges.
2. **Spine** — a thick strip down the center using the novel's spine color. Darker than the cover.
3. **Page layers** — 3 stacked page layers behind the main spread, each slightly lighter cream, creating depth.
4. **Main pages** — two-page spread. Left page shows the novel's **Open Book left-page deco** emoji (faded, decorative). Right page shows the novel title, chapter numbers, and the prompt "Open your book or choose how to read below."
5. **Gutter shadow** — a soft gradient shadow along the center fold.
6. **Page edge lines** — subtle horizontal line textures on both outer edges (stacked pages effect).

The cover color and left-page emoji **must match the current novel's identity**. See the Novel Identity System below.

### Collapsible Intro Section

The Big Question + Objectives + "You'll need" strip are fully expanded on the Warm-Up tab. When the student navigates to any other tab, this section **auto-collapses** to a slim bar showing "Today's Wonder & Objectives ▼ Expand." Students can tap to re-expand. It auto-expands when returning to Warm-Up.

### The Cardinal Rule: No Cross-Tab References

**Never tell students to look at, go back to, or reference content on a different tab than the one they are currently viewing.** Each tab must be self-contained enough that the student never needs to leave it to understand what they're doing.

- ❌ "Look back at the spelling examples on the Word Study tab."
- ❌ "Go to Tab 3 to find the reading link."
- ❌ "Refer to the vocabulary cards on the previous tab."
- ✅ Repeat the key information briefly if it's needed. A 1-sentence recap is always better than sending the student elsewhere.
- ✅ If a spelling rule was introduced on Tab 2 and is needed on Tab 4, restate the rule in 1 sentence on Tab 4.
- ✅ If vocabulary words are needed for a task on Tab 4, list the words again right there.

This rule applies to all student-facing text, including callouts, hints, instructions, and question stems.

---

## Design System

### Novel Identity System

Each novel unit has its own subtle visual identity. When building a lesson, look up the current novel below and apply its accent colors, emoji set, tracker scene, and quote strip. The base template (navy header, tab structure, card styles) stays the same — only these accent elements shift.

**Always check which novel is active before building.** The novel identity affects: accent colors on activity cards and callouts, emoji used in the tracker and throughout, the story journey tracker landscape, and the quote strip below the header.

#### The Witch of Blackbird Pond — by Elizabeth George Speare

| Element | Value |
|---|---|
| **Accent palette** | Colonial blue `#3B5998` + autumn gold `#C7922C` |
| **Accent gradient** | `linear-gradient(135deg, #3B5998, #5A7BC0)` |
| **Emoji set** | 🏛️ 🌊 📜 🕊️ 🍂 🔥 |
| **Character token** | 🕊️ |
| **Tracker scene** | A New England colonial landscape — autumn trees, wooden houses with thatched roofs, a meadow leading to marshland. Landmarks: ⛵ the ship *Dolophin* (start), 🏘️ Wethersfield village, ⛪ the meetinghouse, 🏠 the Wood family house, 🌿 the meadow with cattails, 🏚️ Hannah Tupper's cottage by Blackbird Pond (end). Autumn leaves (🍂) drifting. A duck or two on the pond. Path stroke: `#8B6914` (earthy brown). Background: muted autumn sky, warm golds and blues. |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Colonial, autumn, courage against conformity, warm earth tones and steel blue |
| **Open Book cover** | `linear-gradient(145deg, #2A4278, #3B5998, #4A69A8)` with spine `#1E3060` |
| **Open Book left-page deco** | 🕊️ |

#### Johnny Tremain — by Esther Forbes

| Element | Value |
|---|---|
| **Accent palette** | Revolutionary red `#8B2500` + parchment gold `#D4A843` |
| **Accent gradient** | `linear-gradient(135deg, #8B2500, #A83820)` |
| **Emoji set** | ⚒️ 🔔 📜 🐎 🗽 🔥 |
| **Character token** | ⚒️ |
| **Tracker scene** | Colonial Boston — narrow cobblestone streets, brick buildings, a harbor with ships. Landmarks: ⚒️ the Lapham silversmith shop (start), 🏪 the print shop (Boston Observer), ⛪ the Old North Church, 🏛️ Faneuil Hall, 🐎 the messenger route, 🔔 the Liberty Tree (end). Scattered 📜 pamphlets and colonial lanterns. A harbor with ship masts in the distance. Path stroke: `#8B6914` (cobblestone tan). Background: brick-red and parchment gradient. |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Revolutionary energy, fire and iron, courage and sacrifice, warm reds and golds |
| **Open Book cover** | `linear-gradient(145deg, #6B1A00, #8B2500, #A83820)` with spine `#4A1200` |
| **Open Book left-page deco** | 🔔 |

#### Carry On, Mr. Bowditch — by Jean Lee Latham

| Element | Value |
|---|---|
| **Accent palette** | Ocean navy `#1B3A5C` + compass gold `#C9A84C` |
| **Accent gradient** | `linear-gradient(135deg, #1B3A5C, #2A5080)` |
| **Emoji set** | ⭐ 🧭 📐 🚢 📖 🌊 |
| **Character token** | 🧭 |
| **Tracker scene** | A harbor town with ships and a starry sky. Landmarks: 🏠 the Bowditch home in Salem (start), 📖 the chandlery/bookshop, 🏫 the schoolhouse, 🚢 a merchant ship at the wharf, 🌊 the open ocean, ⭐ a constellation-filled sky (end). Navigation instruments (📐) scattered. A lighthouse. Stars are prominent. Path stroke: `#C9A84C` (compass gold). Background: deep navy to starry sky gradient. |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Starlit navigation, determination through learning, ocean and sky, deep navy and gold |
| **Open Book cover** | `linear-gradient(145deg, #0E2840, #1B3A5C, #2A5080)` with spine `#081E30` |
| **Open Book left-page deco** | ⭐ |

#### Soft Rain — by Cornelia Cornelissen

| Element | Value |
|---|---|
| **Accent palette** | Forest green `#2D6B3A` + clay red `#A0522D` |
| **Accent gradient** | `linear-gradient(135deg, #2D6B3A, #408050)` |
| **Emoji set** | 🌧️ 🌿 🏔️ 🦌 🪶 💧 |
| **Character token** | 🌧️ |
| **Tracker scene** | The Cherokee homeland — Blue Ridge mountains with mist, a village with log cabins and fields. Landmarks: 🏡 Soft Rain's family cabin (start), 🌾 the cornfield, 🏔️ the mountain overlook, 🪶 the council house, 🛤️ the beginning of the trail, 💧 a river crossing (end). Mist and soft rain. Deciduous and evergreen trees. Wildflowers. Path stroke: `#A0522D` (clay red). Background: misty green-blue mountain gradient. |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Quiet grief, connection to land, mist and rain, earthy greens and clay |
| **Open Book cover** | `linear-gradient(145deg, #1E5028, #2D6B3A, #3D8050)` with spine `#143820` |
| **Open Book left-page deco** | 🪶 |

#### How I Became a Ghost — by Tim Tingle

| Element | Value |
|---|---|
| **Accent palette** | Twilight purple `#4A3060` + spirit blue `#6B8FC0` |
| **Accent gradient** | `linear-gradient(135deg, #4A3060, #603E80)` |
| **Emoji set** | 👻 🌙 🔥 🦉 🌌 💫 |
| **Character token** | 👻 |
| **Tracker scene** | A Choctaw landscape at twilight — deep purple sky, firelight, spirit trails. Landmarks: 🏡 Isaac's family home (start), 🔥 the community fire, 🌲 the dark woods, 🦉 the owl perch, 🛤️ the Trail of Tears path, 🌌 the spirit world (end). Spirit wisps (💫) floating. Fireflies. An owl in silhouette. Path stroke: `#6B8FC0` (spirit blue). Background: deep twilight purple to dark sky gradient. Stars and a crescent moon (🌙). |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Haunting and tender, twilight and firelight, between worlds, deep purple and spirit blue |
| **Open Book cover** | `linear-gradient(145deg, #3A2048, #4A3060, #5A4078)` with spine `#2A1838` |
| **Open Book left-page deco** | 🌙 |

#### By the Great Horn Spoon! — by Sid Fleischman

| Element | Value |
|---|---|
| **Accent palette** | Gold rush amber `#D4A020` + adventure brown `#6B4226` |
| **Accent gradient** | `linear-gradient(135deg, #D4A020, #E8B830)` |
| **Emoji set** | ⛏️ 🤠 🚢 💰 🏔️ 🌵 |
| **Character token** | ⛏️ |
| **Tracker scene** | A Gold Rush adventure landscape — ocean, ship, then overland to the mines. Landmarks: 🏠 Aunt Arabella's Boston mansion (start), 🚢 the ship *Lady Dolopin* at sea, 🌊 rounding Cape Horn, 🏖️ arriving in San Francisco, 🏔️ the foothills, ⛏️ the gold mine (end). Scattered 💰 gold nuggets and 🌵 cacti. A pickaxe and pan. Path stroke: `#D4A020` (gold rush amber). Background: warm amber to dusty brown gradient with blue sky. |
| **Quote strip** | A quote from the novel, changed per lesson |
| **Feeling** | Adventure and humor, gold and dust, exuberant energy, warm ambers and browns |
| **Open Book cover** | `linear-gradient(145deg, #B48818, #D4A020, #E8B830)` with spine `#8A6810` |
| **Open Book left-page deco** | 💰 |

---

### ELA Base Colors (always present regardless of novel)

| Role | Color | Hex |
|---|---|---|
| Primary accent | Deep teal | `#00695C` |
| Secondary accent | Warm gold | `#F9A825` |
| Header gradient | Navy (same as science) | `#0E1C42 → #1A2D5A` |
| Tab active border | Teal | `#00695C` |
| Activity warm-up | Sage green | `#52B788` |
| Activity lesson | Gold | `#F9A825` |
| Activity practice | Teal | `#00796B` |
| Activity check | Plum | `#7B5EA7` |
| Back-to-top pill | Teal gradient | `#00695C → #00897B` |
| Progress bar fill | Gold → teal | `#F9A825 → #00897B` |

### Header Badge
- Uses the week/lesson number: **"Lesson 9.1"**
- Emoji: use a book, quill, or letter-themed emoji appropriate to the lesson content.
- No subject label ("ELA" or "English") in the badge — lesson number only.

### Info Strip (below hero banner)
Replace science-specific fields with ELA fields:

| Icon | Label | Value |
|---|---|---|
| 📚 | Unit | Unit name or novel title |
| 📅 | Week | Week number + Lesson number |
| 📖 | Reading | Novel title + chapter(s) |
| 🔤 | Focus | Grammar + Spelling topic |

### Hero Banner SVG
- viewBox: `920 × 260`
- Hand-coded SVG scene — never a placeholder.
- Topic: illustrate something from the novel, the week's theme, or the writing skill.
- Must include 2–3 animations (floating, drifting, pulsing — nothing jarring).
- **No `<text>` elements** — no lesson titles, labels, or captions in the SVG.
- Classical and literary in feeling — think warm light, books, nature, handwriting, ink, candles, gardens, old houses, ships, colonial architecture, mountains, trails.

---

## Classical Pedagogy — Silent Embedding

The ELA lessons must feel **warm, thoughtful, and guided** — like a knowledgeable teacher walking students through great literature. The following classical pedagogy elements must be embedded naturally, without labeling them for students.

**Narration:** After reading a section, ask students to retell or summarize in their own words.
> "In your own words, explain what happened when Kit arrived at the Wethersfield dock."

**Imitation:** Include at least one Writing Connection task per week that asks students to imitate a sentence pattern from the text.
> "Use this sentence as a model: [sentence]. Write your own version about a different character or situation."

**Socratic Questions:** Reading comprehension questions should not all be recall. At least 2 per day should require genuine reasoning:
> "Why does Kit jump into the water to retrieve the doll, even though she knows the Puritans will disapprove? What does this tell us about her values?"

**Evidence Before Explanation:** Students should find something in the text before explaining. Don't ask "What is the theme?" — ask "What detail in this chapter made you think the theme might be about [X]?"

### What NOT to Do
- Don't use terms like "narration," "Socratic," or "imitation" on the student page.
- Don't write objectives in passive voice ("Students will be able to...") — use active verbs only.
- Don't make the lesson feel like a worksheet. Every section should have a brief teacher voice that introduces the task and explains why it matters.
- Don't use AI-sounding filler: "Great job!", "Let's explore!", "In today's lesson, we will..." followed by a bullet list. Write in direct, warm, teacher voice.

---

## Writing Standards

- **Voice:** Warm, direct, knowledgeable. Sounds like a teacher who loves this book and knows these students.
- **Sentence length:** Average ≤ 15 words. No sentence over 25 words. No paragraph over 4 sentences.
- **Total reading per lesson:** 800–1,100 words of student-facing text across all tabs.
- **No references to "the class," "your partner," or "your group."** Students work alone.
- **No passive construction for student tasks.** Write "Copy this sentence" not "This sentence should be copied."
- **Novel references must be accurate** — do not paraphrase chapter content incorrectly. If you don't have access to chapter text, note the specific questions to ask the user.

---

## Back to Top Button

Every lesson must include the full iframe-aware Back to Top button from the science template. Do not simplify it. Use the multi-strategy click handler and `#pageTop` anchor. Button color uses the ELA teal accent.

---

## Progress Bar

One `.progress-wrap` per lesson, at the very top. Tracks tab visits. Progress emoji should match the lesson's theme (📖 for reading-heavy days, ✏️ for writing-heavy days, 🔤 for word-study days).

---

## Confetti

Fires in exactly two places:
1. All turn-in checklist items checked (the Assignment tab).
2. (Optional) Perfect score on any embedded self-check quiz.

---

## Quality Checklist

Before saving any lesson file, confirm:

- [ ] All `✏️` markers replaced — search for any missed fields
- [ ] Objectives use correct arc verb for the day (define / identify / use / explain)
- [ ] Grammar task matches the day's position in the arc
- [ ] **Grammar sentences come from or are inspired by the novel** — no generic sentences
- [ ] Spelling task matches the day's position in the arc
- [ ] **DOL sentences come from or are inspired by the novel** — character names, settings, events
- [ ] **What Good Readers Do** present — Tab 1 on Days 1 & 2; Tab 3 on Days 3 & 4
- [ ] What Good Readers Do strategy matches the novel stage and connects to at least one comprehension question
- [ ] **RWM** present on Days 2 and/or 3 in Tab 2 — sentence pulled from the novel, all three steps present, sentence frame included
- [ ] RWM sentence connects to the week's grammar skill when possible
- [ ] **Weekly Fluency** built as a separate HTML file (`lesson-[week]-fluency.html`), not embedded in the daily lesson
- [ ] **Weekly Check-In** built as a separate HTML file (`lesson-[week]-checkin.html`), not embedded in the daily lesson
- [ ] **No copywork anywhere** — Poetry Corner on Days 2 & 4 only; Days 1 & 3 have DOL only
- [ ] **Poetry Corner** present on Days 2 & 4 with poem, author, and Socratic question
- [ ] **Vocabulary activity** present in Tab 2 every day — format matches the daily rotation (flip cards Day 1, sort Day 2, use it Day 3, choice board Day 4)
- [ ] Vocabulary choice board appears only on Day 4 and is submitted via the Assignment tab
- [ ] **Morphology** includes Root Match mini-game + journal textbox on Days 1–2
- [ ] **Only 5 graded textboxes** in the lesson: 1 Word Study SWYK + 3 comprehension + 1 writing connection
- [ ] Every textbox has a **persistent prompt** above it (`.textbox-prompt`) and a **sentence starter** as placeholder
- [ ] **3 comprehension questions** on the Assignment tab (not more) — each requiring evidence from the text
- [ ] **Day 4 lessons** include at least one reflective question that looks across the week's reading
- [ ] **Interactive mini-games** (3–5 per lesson) all use novel-connected content and track completion in JS variables
- [ ] **No cross-tab references** — no student-facing text says "go back to," "look at the Word Study tab," or "refer to Tab X." Each tab is self-contained. Repeat key info briefly if needed.
- [ ] **Narrative transition** present at the bottom of every tab (Tabs 1–3): italic teacher-voice sentence + continue button
- [ ] **Novel quote strip** present between the info strip and intro cards
- [ ] **"Open Your Book" card** present on Tab 3 before the read/listen links
- [ ] **Collapsible intro section** works: expanded on Warm-Up, collapsed on all other tabs, re-expandable by tap
- [ ] **Today's Path** roadmap present in the collapsible intro (4 steps with arrows)
- [ ] **"Download All My Work" button** present on the Assignment tab, below the turn-in checklist
- [ ] Download captures all journal textbox values + all mini-game completion statuses
- [ ] Video slots: every slot has a correct `<!-- slot: [week]-[day]-[type] -->` comment
- [ ] DOL includes a textbox for corrections + a "Check My Work" reveal button
- [ ] Vocabulary flip cards present on Tab 2, Day 1 (4–6 words), each with the actual novel sentence on the front
- [ ] Reading chapter links present on Tab 3
- [ ] Guided stopping points (2–3 Pause and Think prompts) present on Tab 3 — each with a journal textbox
- [ ] Grammar feedback video slot present after grammar task on Tab 2
- [ ] Spelling feedback video slot present after spelling task on Tab 2
- [ ] Writing Connection present on Tab 4 with a journal textbox (no interactive game — students just write)
- [ ] Reading comprehension questions present and accurate on the Assignment tab
- [ ] Turn-in checklist present with all items including morphology
- [ ] No references to "the class," "your partner," or "your group"
- [ ] At least 2 Socratic-style comprehension questions per chapter
- [ ] Writing sounds like a teacher — not AI-generated filler
- [ ] Back to Top button uses full iframe-aware multi-strategy JS (not simplified)
- [ ] Exactly ONE `.progress-wrap` in the lesson, flush with the tab bar (no gap)
- [ ] Confetti fires only at checklist completion (and optional quiz)
- [ ] File named correctly: `lesson-[week]-[day]-[slug].html`
- [ ] **Weekly check-in** file named correctly: `lesson-[week]-checkin.html`
- [ ] **Assessment expectations match the week** — check the Weekly Check-In Map for focus areas

---

## Common Mistakes to Avoid

- **Don't repeat the same grammar reminder text verbatim across all 4 days.** Each day's reminder should be one sentence — just enough context. The full explanation is on Day 1 only.
- **Don't use generic grammar sentences.** Every grammar example, practice sentence, and DOL sentence must come from or be inspired by the novel. Character names, settings, events — keep it in the story's world.
- **Don't write comprehension questions that can be answered with one word.** Every question should require a sentence.
- **Don't skip the DOL feedback video slot.** Students must always have a way to check their DOL work.
- **Don't put the vocabulary choice board on every tab.** It appears once or twice per week — not on every day.
- **Don't make the hero banner a placeholder.** Build the scene. If you need ideas, ask the user what chapter themes or images stand out.
- **Don't write DOL sentences with invented, implausible errors.** Errors should be realistic (a student might actually make this mistake) and connected to the novel.
- **Don't tell students to look at another tab.** Never say "go back to the Word Study tab" or "see the spelling examples on Tab 2." Restate the needed information briefly on the current tab instead.
- **Don't add interactive writing games (sentence builders, etc.).** Writing tasks should use journal textboxes. Students should just write — the interactives are for recognition and sorting tasks only.
- **Don't forget the Download button.** Every lesson must include the "Download All My Work" button on the Assignment tab. It must capture all journal textbox values and all mini-game completion statuses.
- **Don't include a "draw the word" option** in the vocabulary choice board. All vocabulary activities should involve reading, writing, or explaining — not drawing.
- **Don't put weekly fluency inside a daily lesson page.** Fluency is always a separate HTML file because it requires Canvas's recording tool.
- **Don't put the weekly check-in inside a daily lesson page.** The check-in is always a separate HTML file designed to become a Canvas quiz.
- **Don't include copywork.** There is no copywork in 5th grade ELA. Poetry Corner on Days 2 & 4 is the only warm-up supplement beyond DOL.
- **Don't make Day 4 feel like every other day.** Day 4 is the week closer — at least one comprehension question should look across the full week's reading, and the Writing Connection should be slightly more reflective.
- **Don't leave a gap between the progress bar and tab bar.** The tab bar's `top` value must be set dynamically by JS to match the progress bar height.
- **Don't undersell 5th grade expectations.** Questions, writing tasks, and RWM prompts should push students toward analytical thinking, evidence-based reasoning, and craft awareness. This is not 4th grade — sentence frames should scaffold without over-simplifying.
