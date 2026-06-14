# Skill: AI-Tell Self-Audit

Scan a piece of writing for the words, phrases, and patterns that make text read as AI-generated. Flag every hit, then rewrite it to sound human.

## What to do
1. Read the text the user provides.
2. Flag every match against the lists below. For each, quote the sentence and name the offence.
3. Score the draft: count of banned words + phrases + structural patterns found.
4. Rewrite the flagged sentences in plain human language, keeping the meaning and every fact.
5. Return: the flag list, then the clean rewritten version.

## Banned words (cut or replace every one)
delve, leverage, foster, utilize, navigate, underscore, endeavor, harness, facilitate, optimize, streamline, empower, empowering, ignite, unleash, uncover, elevate, bolster, spearhead, catalyze, resonate, illuminate, encompass, crucial, pivotal, transformative, groundbreaking, robust, comprehensive, seamless, innovative, invaluable, multifaceted, dynamic, cutting-edge, future-ready, nuanced, myriad, paramount, noteworthy, profound, intricate, overarching, meticulous, holistic, landscape (as metaphor), tapestry, realm, testament, paradigm, methodology, stakeholders, synergy, ecosystem (as metaphor), bedrock, cornerstone, catalyst, beacon, pinnacle, nexus, interplay, underpinning, plethora, moreover, furthermore, additionally, consequently, nevertheless, notably, crucially, essentially, correspondingly, henceforth, notwithstanding, conversely, likewise, interestingly, firstly, secondly, lastly, aforementioned, pertaining.

## Banned phrases (delete or rewrite)
"important to note", "worth mentioning", "in today's digital age", "in today's fast-paced", "in today's world", "in the ever-evolving", "ever-evolving landscape", "in an era where", "in the realm of", "plays a vital/crucial/significant role", "serves as a testament", "it can be argued", "at its core", "when it comes to", "in light of recent", "it goes without saying", "needless to say", "at the end of the day", "moving forward", "going forward", "that being said", "with that in mind", "here's the thing", "here's the truth", "here's the kicker", "here's what nobody tells you", "here's what most people miss", "here's where it gets interesting", "let that sink in", "read that again", "let me explain", "let's unpack", "let's break this down", "let's dive in", "let's dive deeper", "let's explore", "the answer might surprise you", "what if I told you", "spoiler alert", "it could be argued", "one might suggest", "while it is true", "this article aims", "aims to explore", "shed light on", "only time will tell", "the jury is still out", "no one-size-fits-all", "it's not about X, it's about Y", "this isn't about", "the question is not", "most people don't realize", "picture this", "imagine this", "have you ever wondered", "published a paper/study/report", "the real question is", "the truth is", "the reality is", "the uncomfortable truth", "the good news is", "gain insights", "offers valuable perspectives", "in conclusion", "to sum up", "to summarize", "all in all", "final thoughts", "the takeaway is clear", "one thing is clear", "the possibilities are endless", "the future is bright", "paves the way", "without further ado", "on the flip side", "in a similar vein", "to that end", "not only... but also".

## Structural patterns (the deeper tells)
- "In [YEAR]," study-introduction openers and "published a paper/study" formulas.
- "The X" sentence starters overused (more than ~20% of sentences).
- Uniform sentence length (everything 15-25 words). Vary it.
- Perfect paragraph rectangles (every paragraph 3 sentences of similar length).
- Correlative pairs overused: "not only... but also", "whether... or", "both... and".
- Same emotional arc in every section: problem -> study -> reframe -> solution.
- "It's not X, it's Y" contrast framing: max one per piece.
- Staccato fragment pairs ("Not anymore." "Until now."): max one per piece.
- Em-dashes and en-dashes everywhere: replace with commas, periods, or a normal hyphen.
- Anaphora: three or more sentences starting with the same word.
- The same statistic repeated three or more times.

## Output
1. Flag report: each hit quoted, with the offence named.
2. A score (total tells found).
3. The rewritten, human version, ready to paste.
