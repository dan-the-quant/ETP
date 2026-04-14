# WOK Audit Framework
## Epistemic Portfolio Theory (EPT) — Daniel Barrera | Dan the Quant

**Version:** 0.1 — Working Draft
**Status:** Open source. Free to use, adapt, and share with attribution.
**Contact:** danthequant.com | Substack | LinkedIn

---

## What This Is

The WOK Audit is a structured checklist for evaluating the epistemological quality of any piece of research, AI-generated output, investment thesis, or quantitative model. It applies the eight Ways of Knowing (WOKs) — drawn from the International Baccalaureate Theory of Knowledge curriculum — as a diagnostic lens.

The audit does NOT replace technical review. It runs alongside it, asking a prior question: by what means does this piece of work claim to know what it claims to know?

The most valuable output of this audit is the qualitative diagnosis — which WOKs are deployed, which are neglected, and where the epistemological weaknesses are. The numerical score is a convenience summary only. See the scoring caveat below.

---

## The Eight Ways of Knowing

| # | WOK | Core Question | Investment / Research Analog |
|---|-----|---------------|------------------------------|
| 1 | Reason | Is the logic valid and internally consistent? | Model construction, DCF, factor logic, hypothesis formation |
| 2 | Sense Perception | What direct evidence grounds this? | Empirical data, price action, observed market behavior |
| 3 | Language | Is the thesis stated precisely enough to be falsified? | Thesis articulation, variable definitions, hypothesis framing |
| 4 | Memory | Does this account for historical precedent and regime context? | Cycle awareness, backtesting across regimes, out-of-sample testing |
| 5 | Imagination | Are tail risks and non-historical scenarios considered? | Stress testing, scenario analysis, regime-change sensitivity |
| 6 | Emotion | Is sentiment or conviction treated as signal or noise? | Contrarian indicators, crowding detection, conviction calibration |
| 7 | Intuition | Is expert pattern recognition acknowledged and examined? | Discretionary overlays, pre-analytical conviction, practitioner judgment |
| 8 | Faith | Is sustained conviction through disconfirmation defensible? | Position sizing during drawdowns, factor thesis holding through adversity |

---

## The Audit Checklist

For each WOK, assess the work on two dimensions:

Deployment: Is this WOK present or absent?
  1 = actively deployed
  0 = absent or ignored

Discipline: If deployed, how well-disciplined is it?
  +1 = deployed rigorously, truth-seeking, falsification-friendly
   0 = deployed but neutrally (present but not examined)
  -1 = deployed but misleading, confirmation-seeking, or actively harmful

---

### WOK 1 — Reason

Checklist:
- [ ] Are the core assumptions stated explicitly?
- [ ] Is the logical chain from assumptions to conclusions valid?
- [ ] Are there internal contradictions between different parts of the argument?
- [ ] Is the reasoning falsifiable — could new data change the conclusion?
- [ ] Are confidence intervals or uncertainty bounds provided where appropriate?

Failure modes: Circular reasoning, overfitting logic to desired conclusion, treating model output as reality, mistaking correlation for causation.

AI-specific risk: AI reasons fluently within its training distribution with no awareness of when it has left it. High Reason scores in AI output do not imply the reasoning is grounded in current or relevant data.

---

### WOK 2 — Sense Perception

Checklist:
- [ ] What direct empirical evidence grounds the core claims?
- [ ] Is the data source identified, dated, and appropriate to the question?
- [ ] Are there data quality issues (survivorship bias, look-ahead bias, selection bias)?
- [ ] Is the observation period representative of the regime being modeled?
- [ ] Have contrary observations been sought, not just confirming ones?

Failure modes: Cherry-picked samples, survivorship bias, conflating statistical fit with predictive validity, treating in-sample results as out-of-sample.

AI-specific risk: AI pattern-matches at scale and returns outputs that feel observational. They are statistical — derived from training data, not from direct market observation.

---

### WOK 3 — Language

Checklist:
- [ ] Is the central thesis stated in a form precise enough to be falsified?
- [ ] Are key terms defined unambiguously?
- [ ] Could a skilled critic identify a specific prediction that, if wrong, would overturn the thesis?
- [ ] Does the language distinguish between what is known, what is assumed, and what is speculated?
- [ ] Are hedges and qualifications proportionate to the actual uncertainty?

Failure modes: Vague hypotheses that cannot be tested, conflating description with prediction, language that performs certainty without substance, thesis drift.

AI-specific risk: AI produces language with authority. Authority is not accuracy. This is the WOK where AI is simultaneously most capable and most dangerous — fluency creates the illusion of precision.

---

### WOK 4 — Memory

Checklist:
- [ ] Does the analysis account for multiple market regimes (not just the training period)?
- [ ] Are historical analogues cited, and are they genuinely analogous?
- [ ] Is the backtest period long enough to include at least one full cycle?
- [ ] Are the results robust across different sub-periods?
- [ ] Does the work acknowledge what was NOT observed in the historical record?

Failure modes: Overfitting to a single regime, recency bias, treating the last decade as representative of all time, ignoring structural breaks.

AI-specific risk: AI has no episodic memory. It treats 2008 dynamics and 2024 dynamics with equal confidence and no sense of which regime the current moment resembles.

---

### WOK 5 — Imagination

Checklist:
- [ ] Are scenarios considered that the historical data has never produced?
- [ ] Is there a mechanism described for how the thesis could fail catastrophically?
- [ ] Are correlation breakdowns in stress scenarios modeled or acknowledged?
- [ ] Is the analysis robust to at least one "this time is different" scenario?
- [ ] Have second-order and third-order consequences been considered?

Failure modes: Anchoring exclusively to historical distributions, treating tail risk as synonymous with historical worst-case, LTCM-style blindness to correlated failure modes.

AI-specific risk: AI generates scenarios readily, but novel-sounding scenarios may be hallucinations. Every AI-generated scenario should be grounded in a historical analogue, a mechanism, and a falsifiable prediction before it enters a model.

---

### WOK 6 — Emotion

Checklist:
- [ ] Is collective sentiment identified as a variable (not ignored)?
- [ ] Is the author's own conviction examined for potential bias?
- [ ] Is there a mechanism for distinguishing genuine contrarian signal from premature positioning?
- [ ] Are there explicit rules for when emotional signal constitutes a buy or sell indicator?
- [ ] Is crowding or herding risk addressed?

Failure modes: Dismissing sentiment data as "soft," ignoring crowding risk, mistaking enthusiasm for edge, holding through drawdown due to emotional attachment rather than thesis integrity.

AI-specific risk: AI has no emotional stake in the outcome — which sounds like an advantage until you realize it also has no alarm system. It will not feel that something is wrong.

---

### WOK 7 — Intuition

Checklist:
- [ ] Is practitioner judgment or pattern recognition used — and if so, is it named?
- [ ] Is the intuition based on documented experience or undifferentiated gut feel?
- [ ] Has the intuitive signal been stress-tested against explicit criteria?
- [ ] Is there a record of past intuitive calls and their outcomes (feedback loop)?
- [ ] Is the intuition distinguished from bias or motivated reasoning?

Failure modes: Passing off unexamined bias as expert pattern recognition, dismissing intuition entirely, overconfident intuition with no feedback calibration.

AI-specific risk: AI produces outputs that feel intuitive to the reader. That feeling is the reader's own intuition being triggered by the AI's fluency — it is not the AI having intuition. These are categorically different things.

---

### WOK 8 — Faith

Checklist:
- [ ] Is there a clearly stated falsification threshold — at what point does the thesis fail?
- [ ] Is sustained conviction during drawdown based on thesis integrity or sunk cost?
- [ ] Is the holding period justified by the thesis logic, not by hope?
- [ ] Has the thesis been stress-tested against the specific conditions under which it historically fails?
- [ ] Is the conviction level (position sizing) proportionate to the epistemic quality of the thesis?

Failure modes: Holding through legitimate disconfirmation, abandoning sound thesis at first drawdown, ideological attachment to a factor or framework beyond its empirical support.

AI-specific risk: AI has no convictions. But it will enthusiastically reinforce yours if asked to defend a thesis — and will do so with equal fluency whether the thesis is right or wrong. Explicitly task AI to destroy your thesis, not just support it.

---

## SCORING CAVEAT — READ BEFORE USING THE SCORE

The numerical score below is a first-pass heuristic, not an empirically validated measure. It is naive, has not been tested against investment outcomes, and should not be treated as a reliable ranking system. The score's primary value is to force a structured traversal of all eight dimensions — the number itself is a convenience summary that may be refined or replaced entirely as the framework develops.

The most valuable output of this audit is the qualitative diagnosis: which WOKs are deployed, which are neglected, where the failure modes are most likely, and what questions the work leaves unanswered. Trust that. Treat the score as a rough orientation, not a verdict.

---

## Scoring (Tentative — Under Construction)

WOK Score = Deployment x Discipline

For each WOK:
  Absent (0) x n/a              =  0
  Present (1) x Rigorous (+1)   = +1
  Present (1) x Neutral (0)     =  0
  Present (1) x Misleading (-1) = -1

Aggregate Score = sum of all eight WOK scores, divided by 8
Range: -1 (epistemologically bankrupt) to +1 (exceptional)

Illustrative benchmarks (not statistically validated):
  +0.70 to +1.00  Exceptional epistemic diversity
  +0.40 to +0.69  Solid — some WOKs underdeveloped
  +0.10 to +0.39  Adequate but significant gaps
  -0.10 to +0.09  Compromised — serious epistemological problems
  Below -0.10     Deeply problematic

---

## Application Notes

For investment research papers:
Apply the checklist to each WOK. Note absences as carefully as presences — a paper that deploys Reason and Perception rigorously but ignores Imagination and Memory is telling you something important about its limits.

For AI-generated outputs:
AI systematically over-indexes on Reason and Language while producing near-zero authentic Perception, Memory, Intuition, Emotion, and Faith. Use the audit to identify which WOKs are missing and supplement accordingly.

For your own work:
Auditing your own research is the most valuable and most uncomfortable application. The first audit in this framework was applied to the framework itself. Start there.

For team processes:
Epistemological clashes between team members often present as personality conflicts. The WOK audit gives them a shared vocabulary for that conversation.

---

## Philosophical Lineage

- Reason: Aristotle, Descartes, Kant
- Sense Perception: Locke, Hume, Russell
- Language: Wittgenstein, Austin, Chomsky
- Memory: Bergson, Tulving
- Imagination: Kant, Bachelard, Sartre
- Emotion: William James, Damasio, Feldman Barrett
- Intuition: Bergson, Klein, Gigerenzer
- Faith: William James, Plantinga, Tillich

The application of WOKs to investment decision-making and AI evaluation is original to Epistemic Portfolio Theory (EPT), developed by Daniel Barrera.

---

## Citation

Barrera, D. (2026). WOK Audit Framework: Epistemic Portfolio Theory. Working document. danthequant.com
