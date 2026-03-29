# ✍️ WriteRight Chennai — Claude Skill

> **Plagiarism checker + AI detector + student voice rewriter — built for Indian college students.**

Paste your essay. Get a plagiarism report. Get a clean rewrite that sounds like *you* — a real South Indian college student, not a robot.

---

## What it does

Most rewriting tools either sound too polished (obviously AI) or too broken (bad spinner). This skill does something different: it rewrites your text to sound like a genuine **Chennai college student writing at IELTS Band 6.5** — confident, direct, slightly imperfect in the right places, with real opinions and Indian English patterns.

### Full pipeline in one shot:

| Step | What happens |
|------|-------------|
| 🔍 **Detect** | Scans for plagiarism signals AND AI tells — tonal shifts, patchwork writing, AI vocabulary, suspicious structure |
| 🚩 **Flag** | Shows exactly which lines are risky and why, with 🔴🟡🟢 risk scores per segment |
| ✍️ **Rewrite** | Transforms into your voice — Tamil-influenced English, real opinions, natural small slips, Chennai anchors |

### Three modes:
- **"Check this"** → plagiarism + AI detection report only
- **"Rewrite this"** → straight to student voice rewrite
- **"Check and fix"** → full pipeline (default when unsure)

---

## Who this is for

- 🎓 College students in Chennai — Anna University, SRM, VIT, Loyola, MCC, and affiliated colleges
- 📚 Indian students broadly who write assignments in English as a second language
- 🌍 Anyone using Claude who wants to humanize AI-generated text
- 📝 IELTS test takers targeting Band 6–7 writing style

---

## The voice it writes in

The rewrite sounds like a **real 20-year-old from Chennai**:
- Grew up speaking Tamil at home, learned English in school
- Direct and confident — gets to the point, no unnecessary padding
- Has actual opinions: *"Honestly, I think this approach has more problems than benefits"*
- Natural Tamil-English patterns: *"This is the main issue only"*, *"Chennai itself is proof of this"*
- Grounded in student life: OMR traffic, Chennai summer heat, exam panic, placement season
- IELTS Band 6.5 level: mostly correct, with believable minor slips like dropped articles and preposition quirks

---

## How to install

### Prerequisites
- A [Claude.ai](https://claude.ai) account (Free or Pro)
- Skills must be enabled in your Claude settings

### Steps

1. **Download** the `writeright-chennai.skill` file from this repo (go to [Releases](../../releases) or download directly)

2. **Open Claude.ai** → go to **Settings**

3. **Find the Skills section** → click **"Add Skill"** or **"Upload Skill"**

4. **Upload** the `.skill` file

5. **Done.** Start a new chat and paste any text with a prompt like:
   - *"Check this for plagiarism and rewrite it"*
   - *"Make this sound like me — Chennai student style"*
   - *"Will this pass Turnitin? Fix it."*
   - *"Humanize this essay"*

---

## Example

**Input (AI-generated):**
> Climate change stands as one of the most pivotal challenges of our era, underscoring the urgent need for collective action. Experts argue that without meaningful intervention, the consequences could be catastrophic.

**Output (WriteRight Chennai):**

```
📋 PLAGIARISM & AI DETECTION REPORT
Overall Originality Score: 25% | Risk: 🔴 High

Flagged: "stands as", "pivotal", "underscoring", "Experts argue" — heavy AI vocabulary + vague attribution
```

> Climate change is getting more serious every year and honestly, we can already feel it. Chennai summers are becoming unbearable — that itself is enough proof. Scientists have been warning about this for a long time, but governments are still moving very slowly. It is really frustrating. In my opinion, the time for only talking is over.

---

## Prompt cheat sheet

Once installed, just say any of these in Claude:

```
"Check this for plagiarism"
"Is this copied / AI-written?"
"Rewrite this in Chennai student style"
"Make this sound like a real student"
"Humanize this for my assignment"
"Will this pass Turnitin?"
"Check and rewrite this essay"
"Make it less AI, more me"
"IELTS Band 6.5 rewrite"
```

---

## Files in this repo

```
writeright-chennai/
├── README.md               ← you are here
├── writeright-chennai.skill ← install this in Claude
└── SKILL.md                ← skill source (readable, editable)
```

---

## Want to contribute or remix?

The `SKILL.md` file is fully readable — it's just markdown. You can:
- Fork this repo and edit the persona (different city, different IELTS band)
- Add more Chennai-specific examples
- Submit a PR with improvements

---

## License

MIT — free to use, share, and modify. Credit appreciated but not required.

---

## Made by

A Chennai student, for Chennai students. 🏙️☕

*If this helped you, star the repo — it helps others find it.*
