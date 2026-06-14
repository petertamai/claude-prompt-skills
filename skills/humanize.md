# Skill: Humanize Writing

Rewrite text so it reads like a specific human wrote it, not a language model. This is not a thesaurus pass. It targets the exact, measurable features that detectors and readers use to tell AI from human writing. Keep every fact and the writer's meaning.

---

## How to use
The user gives you text. You return the rewritten version, then a short note on what you changed and why. Do not add information, opinions, or fake specifics the user did not provide. If a sentence needs a concrete detail to feel human, mark it [add specific] rather than invent one.

---

## The evidence this skill runs on
AI text is detectable because it is statistically distinct from human text on a handful of features. Fix the features and you fix the "feel".

1. **Burstiness: humans vary sentence length, AI does not.** Corpus studies of GPT-4 / Claude vs human writing (and the stylometry+perplexity detector literature, F1 ~0.94) consistently find LLMs cluster sentences in the 10-30 word range, while human writing has a much wider spread, very short sentences next to long ones. Low variation is the single loudest AI tell. → Force variance. Put 3-word sentences next to 20-word ones. Never a run of same-length lines.
2. **Perplexity: humans make less predictable word choices.** AI text has low perplexity, the next word is usually the statistically obvious one. Humans pick words for rhythm, memory, and specificity that a model would not predict. → Replace generic words with the precise, concrete one a person who lived it would use. Specific beats smooth.
3. **Excess-vocabulary markers.** Kobak et al. (2024), measuring excess word frequency across 14.2 million PubMed abstracts, found a sharp post-ChatGPT surge in a specific set of words: delve, pivotal, intricate, showcasing, realm, underscore, and similar. These are statistical fingerprints. → Cut them entirely (full list below).
4. **Processing fluency favours simple, concrete language.** Oppenheimer (2006) and the PNAS word-familiarity study (2021): simpler, more familiar words read as more credible and get more engagement. → Plain words beat erudite ones. This aligns with removing the marker words, which are mostly fancy synonyms for simple ideas.
5. **Structural tells.** Beyond words, AI writing repeats shapes: the "it's not X, it's Y" frame, tidy rule-of-three lists, paragraphs of identical length, and the em-dash everywhere. Humans are messier. → Break the shapes.

---

## Operating rules

### 1. Rebuild the rhythm (burstiness)
- After rewriting, the passage must contain at least one very short sentence (under 5 words) and at least one long one (15+). No three consecutive sentences of similar length.
- Read it as if aloud. If it marches in a steady beat, break a sentence in two or fuse two into one.

### 2. Raise the perplexity (word choice)
- Swap generic, predictable words for the specific one. "Things improved" becomes the actual change. "A lot of people" becomes who.
- Keep one or two slightly unexpected, plain word choices that a real person would use. Do not make it weird, make it specific.

### 3. Cut the marker words (delete or replace every one)
delve, leverage, foster, utilize, navigate, underscore, harness, facilitate, optimize, streamline, empower, unleash, uncover, elevate, bolster, spearhead, resonate, illuminate, encompass, showcasing, crucial, pivotal, transformative, groundbreaking, robust, comprehensive, seamless, innovative, invaluable, multifaceted, dynamic, cutting-edge, nuanced, myriad, paramount, intricate, meticulous, holistic, realm, tapestry, testament, paradigm, synergy, ecosystem (as metaphor), cornerstone, beacon, plethora, moreover, furthermore, additionally, consequently, nevertheless, notably, essentially, firstly, secondly, lastly.

### 4. Kill the phrase tells (delete or rewrite)
"it's not X, it's Y", "in today's world", "in the ever-evolving", "when it comes to", "at the end of the day", "needless to say", "it's important to note", "here's the thing", "let that sink in", "the truth is", "in conclusion", "to sum up", "the takeaway is clear", "plays a vital role", "shed light on", "what if I told you", "let's dive in".

### 5. Break the structural shapes
- No "it's not X, it's Y" framing (max zero in short text).
- No rule-of-three in every paragraph. Break the pattern.
- Vary paragraph length. One-line paragraphs are fine and human.
- Replace em-dashes and en-dashes with commas, periods, or a normal hyphen.

### 6. Add quiet human signals
- Use contractions (it's, didn't, here's) where natural.
- Keep the writer's point of view and any first-person voice.
- A little asymmetry is good. Real writing is not perfectly balanced.
- Do NOT add slang, jokes, or personality the original did not have. Humanize the texture, not the meaning.

---

## Process
1. Read the text. Note its current rhythm (are sentences all similar length?) and scan for marker words and phrase tells.
2. Rewrite sentence by sentence: cut markers, swap generic words for specific ones, vary the lengths.
3. Pass back through for rhythm: confirm the short-and-long variance is actually there.
4. Final scan: zero marker words, zero phrase tells, zero em-dashes, no repeated structural shape.

## Self-check before delivering
- [ ] Is there at least one sub-5-word sentence AND one 15+ word sentence? (burstiness)
- [ ] No run of 3+ similar-length sentences?
- [ ] Zero marker words and zero phrase tells from the lists?
- [ ] Generic claims replaced with concrete specifics (or marked [add specific])?
- [ ] No "it's not X, it's Y", no em-dashes, no uniform rule-of-three?
- [ ] Meaning and every fact preserved, nothing invented?

## Output
1. The rewritten text, ready to paste.
2. A two or three line note: what the main tells were and what you changed (e.g. "cut 4 marker words, broke 3 uniform sentences, removed 2 em-dashes").

Do not explain the theory unless asked. Deliver the rewrite.
