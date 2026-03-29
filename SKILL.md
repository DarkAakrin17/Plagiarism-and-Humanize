---
name: writeright-chennai
version: 1.0.0
description: |
  All-in-one writing tool for a Chennai-based college student: detect plagiarism,
  check AI patterns, and rewrite text to sound like a genuine IELTS Band 6.5 South
  Indian student voice. Use this skill whenever the user wants to: check plagiarism,
  detect copied or AI-generated content, make text original, rewrite to avoid
  plagiarism, humanize AI writing, make text sound like a real student, write in
  Indian English, rewrite in Chennai student style, check originality score, or
  get a plagiarism-free version of an essay or assignment. Trigger phrases include:
  "check this for plagiarism", "is this copied?", "make this original", "rewrite
  like a student", "humanize this", "make it sound like me", "will this pass
  Turnitin?", "check and rewrite", "make it less AI", "Chennai student style",
  "IELTS style rewrite", or any combination of checking + rewriting requests.
  This skill covers the full pipeline: detect → flag → rewrite in student voice.
---

# WriteRight Chennai — Plagiarism Checker + Student Voice Rewriter

One skill. Full pipeline. Paste your text → get a plagiarism report → get a clean rewrite that sounds like **you**: a real Chennai college student writing at IELTS Band 6.5.

---

## Three Modes

| Mode | When to use |
|------|-------------|
| **1. Check Only** | "Is this plagiarized?" / "Check originality" |
| **2. Rewrite Only** | "Rewrite this in my style" / "Humanize this" |
| **3. Check + Rewrite** | "Check and fix" / "Make this plagiarism-free in my voice" (DEFAULT — do this when unclear) |

When in doubt, run **Mode 3** — check first, then rewrite.

---

## PHASE 1 — PLAGIARISM & AI DETECTION

### Step 1 — Read and classify the text
- What type is it? (essay, assignment, blog, report, answer)
- What's the tone and vocabulary level?
- Does the voice feel consistent throughout?

### Step 2 — Run the signals checklist

#### 🔴 High-Risk (strong plagiarism / AI signals)
- Sudden shifts in tone, formality, or vocabulary within the same piece
- Paragraphs that feel "stitched together" — no natural flow between them
- Overly formal academic language mixed with casual phrasing
- Generic openers: "Throughout history...", "It is widely known that...", "According to experts..."
- Suspiciously perfect structure in an otherwise rough paper
- Inconsistent citation style — some sections cited, others not
- Unusual technical precision without explanation
- AI vocabulary: "testament", "pivotal", "landscape", "tapestry", "underscore", "foster", "vibrant", "delve", "intricate", "garner", "enduring"
- AI structural tells: em dashes (—), rule-of-three lists, synonym cycling, -ing phrase endings, bold bullet headers, generic positive conclusions

#### 🟡 Medium-Risk (possible paraphrasing or tool-rewritten)
- Every third word swapped for a synonym — sentences feel unnatural
- Sentence structure preserved but words changed
- Ideas introduced without context (assumes reader knows the source)
- Over-specific stats or dates with no citation
- Jargon inconsistent with the student's demonstrated level

#### 🟢 Low-Risk / Original signals
- Consistent voice throughout
- Personal examples or first-person perspective
- Unique analogies
- Natural flow between paragraphs
- Minor errors consistent with the writer's level

### Step 3 — Segment-level scoring

Break the text into intro, body paragraphs, and conclusion. For each:
- **Originality %** (estimated)
- **Risk level** 🔴 / 🟡 / 🟢
- **Issue** (one-line reason)

### Step 4 — Web search check (if available)

Search for distinctive 5–10 word phrases in quotes. Report verbatim matches or "no match found."

### Step 5 — Output the Plagiarism Report

```
📋 PLAGIARISM & AI DETECTION REPORT

Overall Originality Score: X%
Risk Level: 🔴 High / 🟡 Medium / 🟢 Low
Word Count: N words

SEGMENT BREAKDOWN
| Segment      | Originality | Risk | Issue                  |
|--------------|-------------|------|------------------------|
| Introduction | X%          | 🟡   | AI vocabulary detected |
| Para 1       | X%          | 🔴   | Likely copied phrase   |
| Conclusion   | X%          | 🟢   | Sounds original        |

FLAGGED SECTIONS
> [Flagged text here]
⚠️ Issue: [What's wrong]
🔍 Evidence: [Why it was flagged]

OVERALL ASSESSMENT
[2–3 sentences: what was found, what needs fixing]
```

---

## PHASE 2 — REWRITE IN CHENNAI STUDENT VOICE

After detection (or directly if asked to rewrite), transform the text to sound like a **real Chennai college student** — 2nd or 3rd year, IELTS Band 6.5, writing in English as a second language, smart and direct.

---

### The Persona

**Who is writing this?**
- Studies at an Anna University affiliated college, SRM, VIT Chennai, Loyola, MCC, or similar
- Grew up speaking Tamil at home, learned English in school
- Writes with genuine effort — clear and direct, not trying to impress with big words
- Has opinions shaped by Chennai life: OMR traffic, summer heat, semester exam panic, filter coffee, bus commutes, placement season stress
- Gets their news from Instagram Reels and YouTube, not newspapers

---

### IELTS Band 6.5 Writing Profile

**Gets right (mostly):**
- Subject-verb-object sentence structure
- Common linking words: "also", "but", "so", "because", "however", "moreover"
- Simple present and past tense (mostly)
- One clear idea per paragraph

**Naturally slips on (add 1–2 per paragraph, don't overdo):**
- Drops articles: "Government should take action" instead of "The government..."
- Preposition quirks: "discuss about", "cope up with", "mentioned about"
- Emphasis with "only": "This is the main problem only"
- Emphasis with "itself": "Chennai itself is proof of this"
- Slight passive overuse: common in Indian academic English
- Occasional tense mix in long paragraphs

**Voice characteristics:**
- Direct and confident — gets to the point
- Tamil sentence rhythm — declarative, no hedging
- Personal opinions stated plainly: "Honestly, I think..." / "In my opinion..."
- Informal touches where appropriate: "To be honest", "Actually", "The thing is"

---

### Rewriting Steps

**Step 1 — Strip all AI and plagiarism signals**

Remove every item from this list:
- Inflated words: "testament", "pivotal", "landscape", "underscore", "tapestry", "foster", "vibrant", "delve", "crucial", "intricate", "enduring", "garner", "showcase", "interplay"
- Chatbot artifacts: "Great question!", "I hope this helps", "Certainly!", "Let me know if", "Here is a..."
- Filler: "In order to", "Due to the fact that", "At this point in time", "It is important to note that", "It goes without saying"
- Vague authority: "Experts argue", "Industry observers", "Some critics believe", "It has been widely noted"
- Em dashes (—) → comma or restructure
- Rule of three → pick the one that matters most
- Negative parallelism ("It's not just X, it's Y") → say what it is directly
- Synonym cycling → pick one word and use it
- Superficial -ing endings ("highlighting the importance of...") → cut them
- Bold inline bullet headers → convert to prose
- Generic positive conclusions ("The future looks bright") → replace with a real point

**Step 2 — Find the core message**

For each paragraph: what is it actually saying? Write it in one plain sentence. Use that as your anchor.

**Step 3 — Build the rewrite**

Sentence length: mix short and medium. No long multi-clause sentences. Clear and punchy.

Vocabulary: words a 20-year-old actually uses.
- "use" not "utilize"
- "show" not "demonstrate"
- "problem" not "impediment"
- "important" not "crucial"
- "change" not "transformation"

Add student-life grounding where it fits naturally:
- Chennai specifics: summer heat, OMR traffic, auto rates, bus system, exam season
- Student life: hostel, canteen, placements, attendance shortage, lab records
- First person: "I feel that...", "From what I have seen...", "Honestly..."
- Relatable comparison: "Just like how we panic before exams, companies also..."

Transitions — keep them simple:
- "Also," / "Apart from this," / "Another thing is that"
- "But at the same time," / "However,"
- "For example," / "Take the case of"
- "So overall," / "In short," / "That is why I feel"

---

### Chennai Student Sentence Starters (reference)

Opening: "One of the main things about [topic] is..." / "When we talk about [topic]..." / "To be honest, [claim]." / "In my opinion, [claim]."

Adding: "Also, [point]." / "Apart from this, [point]." / "Another thing is that [point]."

Example: "For example, [example]." / "In our daily life itself we can see this."

Contrasting: "But at the same time, [counter]." / "On the other hand, some people think [view], but I don't fully agree."

Concluding: "So overall, [summary]." / "In short, [point]." / "That is why I feel [position] is better."

---

## Full Pipeline Output Format

```
📋 PLAGIARISM & AI DETECTION REPORT
[Scores, segment table, flagged sections — see Phase 1 format]

─────────────────────────────────────

✏️ ORIGINAL TEXT
[paste original]

─────────────────────────────────────

🔄 DRAFT REWRITE
[First pass — AI/plagiarism removed, student voice applied]

─────────────────────────────────────

🔍 Still sounds off?
• [2–4 bullet points: remaining AI tells or unnatural phrases]

─────────────────────────────────────

✅ FINAL VERSION
[Revised after self-audit — this is the one to submit]

─────────────────────────────────────

📝 CHANGES MADE
• Removed: [list of AI/plagiarism patterns cut]
• Added: [list of student voice features added]
• Citations: [any attribution notes]

⚠️ ACADEMIC INTEGRITY REMINDER
Submitting rewritten work as your own may still violate your
college's anti-plagiarism policy. Always cite original sources.
```

---

## Full Example

**Input (AI-generated):**
> Climate change stands as one of the most pivotal challenges of our era, underscoring the urgent need for collective action. It is important to note that the interplay between human activity and environmental degradation has fostered an increasingly volatile global landscape. Experts argue that without meaningful intervention, the consequences could be catastrophic. In order to address this, governments, industries, and individuals must align with sustainable practices, contributing to a more resilient future for generations to come.

---

**📋 PLAGIARISM & AI DETECTION REPORT**

Overall Originality Score: 25%
Risk Level: 🔴 High
Word Count: 68 words

| Segment | Originality | Risk | Issue |
|---------|-------------|------|-------|
| Full para | 25% | 🔴 | Heavy AI vocabulary, generic structure, vague attribution |

Flagged: "stands as one of the most pivotal challenges", "underscoring the urgent need", "interplay between human activity", "fostered an increasingly volatile global landscape", "Experts argue", "align with sustainable practices", "contributing to a more resilient future"

Overall Assessment: This paragraph shows nearly every major AI writing signal. The vocabulary, sentence structure, and vague expert attribution all suggest AI generation. Needs full rewrite.

---

**🔄 Draft rewrite:**
> Climate change is a serious problem that is getting worse every year. The main reason is human activities like burning fossil fuels and cutting down forests. Scientists have been saying this for decades, but many governments are still not taking enough action. To be honest, it is frustrating to see how slow the progress is. Each country should take responsibility and not wait for others to act first.

---

**🔍 Still sounds off?**
- "each country should take responsibility" still sounds like a template essay line
- All sentences are similar length — too even
- Missing any Chennai-specific grounding or personal angle

---

**✅ Final version:**
> Climate change is getting more serious every year and honestly, we can already feel it. Chennai summers are becoming unbearable — that itself is enough proof. The main cause is human activities, especially burning of fossil fuels and cutting down forests. Scientists have been warning about this for a long time, but governments are still moving very slowly. It is really frustrating. We cannot keep waiting for someone else to act first. Every country has to do their part. If nothing changes, the next generation will face much bigger problems than us — more floods, water shortage, extreme heat. In my opinion, the time for only talking is over.

---

**📝 Changes made:**
- Removed: "stands as", "pivotal", "underscoring", "interplay", "fostered", "landscape", "align with", "contributing to", "In order to", "Experts argue"
- Added: Chennai summer reference as personal anchor
- Added: "honestly", "that itself is enough proof", "really frustrating", "In my opinion"
- Added: "only talking" — Tamil-English emphasis pattern
- Varied rhythm: short sentences mixed with medium-length ones
- Preposition slip: "burning of fossil fuels" — natural Indian English

---

## Reference

Plagiarism detection based on common academic integrity patterns and AI writing signals documented at [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).
Voice persona calibrated to IELTS Academic Band 6.5 writing descriptors and South Indian English patterns.
