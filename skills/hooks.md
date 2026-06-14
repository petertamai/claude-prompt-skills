# Skill: Hook Writer

Write the first one or two lines of a LinkedIn post: the only text that shows before "see more", and the single biggest lever on whether anything else gets read. This is an operating manual grounded in the research on attention, curiosity, and clicks. Generate 10 hooks, score them, rank them.

---

## How to use
The user gives you a topic, a draft, or a finished post. You return 10 hooks across different mechanisms, each inside the preview window, each scored, with the top 3 marked. If the topic is vague, ask what the single point is and who it is for before generating. Never invent facts or numbers the user did not supply; if a hook needs a number, mark it [your number].

---

## The evidence this skill runs on
1. **A hook is an information gap, and the gap has a sweet spot.** Loewenstein's information-gap theory (Psych Bulletin, 1994) plus the large-scale test in Scientific Reports (2024), a meta-analysis of 8,977 headline experiments on the Upworthy archive: curiosity is curvilinear. Too vague and the reader feels no gap; too concrete and the gap is already closed, so there is no reason to click. → Reveal enough to make the missing piece felt, withhold the resolution. Name the subject, hide the answer.
2. **Stakes and tension out-pull positivity.** Robertson et al. (Nature Human Behaviour, 2023), a randomised trial across ~105,000 headline variants and 5.7 million clicks, found each additional negative word in an average headline raised click-through by ~2.3%, while positive words lowered it. → Lead with the problem, the cost, the risk, or what breaks, not the happy outcome. (Honesty caveat: that data is news headlines. On professional LinkedIn, pure doom backfires; use *tension and stakes*, not negativity for its own sake.)
3. **People scan; the first words carry the weight.** Nielsen's eye-tracking work (NN/g, 232 users) shows readers scan in an F-pattern and fixate the first two to three words of a line far more than the rest. → Front-load the hook. The most important word goes first, never after a wind-up like "I wanted to share".
4. **Specifics and numerals stop the eye.** Concreteness effect (Paivio) plus industry headline data (Conductor reported ~73% lift, Moz ~15% from numbers; these are vendor studies, not peer-reviewed, treat as directional). Numerals ("7") interrupt a text feed better than spelled words ("seven"); single, specific numbers read as credible. → Use a real, specific number where the material has one.
5. **High-arousal emotion drives sharing.** Berger & Milkman (J. Marketing Research, 2012): awe, anger, anxiety, and amusement transmit; low-arousal calm does not. → Each hook should carry one activating emotion.

## The platform constraint
- The hook must land inside **~210 characters on desktop, ~140 on mobile**, before "see more" cuts it. Write so the cut lands on a cliffhanger, not mid-word.
- Best hooks are usually **one or two short lines**. If it needs three lines to make sense, it is too long.

---

## The hook mechanisms (generate across these, do not use one twice)
Each is a way to open the gap. Pick the ones the user's material can support honestly.
1. **Contrarian** — state the belief everyone holds, signal you are about to break it. ("Most LinkedIn advice is written by people who have never sold anything.")
2. **Specific number / result** — a real, concrete figure that implies a story. ("I sent 100 cold DMs. 3 replied. Here is what the 3 had in common.")
3. **Stakes / cost** — name what is being lost or risked (the negativity-lever, used as tension). ("The slowest way to kill a deal is a 'quick call to align'.")
4. **Confession** — admit a mistake or an uncomfortable truth (vulnerability lowers the reader's guard). ("I lost a 40k client because of one email. My fault entirely.")
5. **Mid-action** — drop the reader into the middle of a scene, no setup. ("Three minutes before the demo, the whole app went blank.")
6. **Direct question** — a question the target reader is privately asking. (Use sparingly; weakest of the set.)
7. **Pattern interrupt** — a short, jarring line that breaks feed rhythm. ("Stop optimising your LinkedIn headline.")

## Calibration rules (apply to every hook)
- **Gap, not summary.** If the hook gives away the payoff, rewrite it. If it reveals nothing, add one concrete detail so the reader feels what is missing.
- **First word earns its place.** Cut greetings, "I", "In today's", "I'm excited to", "Unpopular opinion". Start on the strongest noun, number, or verb.
- **One idea, one emotion.** No stacking.
- **Concrete over abstract.** Real numbers, real things, real moments.
- **No banned AI tells:** "Here's the thing", "Let that sink in", "What if I told you", "Picture this", "The truth is", "Plot twist". No em-dashes.

## Process
1. Identify the one point and the target reader.
2. Pull the concrete assets the user has: numbers, the mistake, the scene, the contrarian belief.
3. Generate 10 hooks spread across at least 6 mechanisms above. Each inside ~210 characters.
4. Score each hook 1-5 on three axes: **Gap** (does it make me need the rest?), **Specificity** (concrete vs vague), **Stakes/emotion** (is there tension?). Sum to /15.
5. Rank them. Mark the top 3. For the top 3, add a one-line note on why it works and which mechanism it uses.

## Output
- A numbered list of 10 hooks.
- Each with its mechanism tag and its /15 score.
- The top 3 flagged, each with a one-line rationale.
- One note if any hook needs a real number the user must fill in ([your number]).

Do not explain the theory unless asked. Deliver the hooks.
