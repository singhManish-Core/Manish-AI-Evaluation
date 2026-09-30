# Interview Defense — Project 01

## 1. Explain the project in 60 seconds.

"I built an independent LLM response-quality benchmark to demonstrate practical AI evaluation skills. I created a controlled prompt set and a six-dimension rubric covering accuracy, reasoning, relevance, completeness, instruction following and clarity. I evaluated response pairs independently, tagged failure modes, recorded evidence for difficult judgments and then made pairwise preference decisions. The goal was to show that I can apply consistent evaluation criteria and explain why one response is better, rather than simply saying that one answer sounds better."

## 2. Why did you choose these six dimensions?

Explain the relationship between correctness, reasoning, task completion and communication. Accuracy and reasoning receive higher weights because a fluent answer can still be wrong.

## 3. Why use weighted scoring?

Because not all quality dimensions have equal impact. The weighting is a study-design choice, not an objective universal truth. State the weights explicitly and discuss how conclusions could change under a different weighting.

## 4. How do you evaluate factuality?

Separate factuality from style. Identify the claim, verify it using an appropriate source when needed, and record the evidence and severity.

## 5. What is hallucination?

A generated claim presented as factual that lacks adequate support or is contradicted by reliable evidence. Be precise about what was actually observed.

## 6. How do you avoid evaluator bias?

Use a predefined rubric, score responses independently before pairwise comparison, document evidence, apply the same criteria to both responses, and record limitations.

## 7. What if both responses are bad?

Do not force a winner. Use "Neither / both materially deficient" when the evaluation protocol permits it, and explain why.

## 8. What if one answer is longer?

Length is not a quality criterion by itself. Evaluate whether the additional content improves completeness and reasoning or creates irrelevant verbosity.

## 9. What if the model sounds confident?

Confidence is not evidence. Unsupported certainty should not receive an accuracy bonus.

## 10. What did you personally contribute?

The portfolio claim should be limited to what you actually did: prompt design, rubric design, response collection, verification, scoring, error analysis and documentation.

## 11. Why is this relevant to AI training work?

It demonstrates transferable evaluator capabilities: structured judgment, instruction-following analysis, factuality checking, comparative ranking, error identification, written justification and consistency.

## 12. What are the limitations?

Discuss sample size, evaluator subjectivity, model/version drift, prompt sensitivity and verification limitations.

## Cross-question drill

Be ready to answer:

- Give an example of an instruction-following failure.
- Give an example where a fluent response was factually weak.
- Which rubric dimension was hardest to score and why?
- How would you improve inter-rater reliability?
- How would you scale from 50 prompts to 5,000?
- How would you evaluate two answers when neither is fully correct?
- How would you detect outdated information?
- How would you handle ambiguous prompts?
- How would you distinguish omission from hallucination?
- How would you design a rubric for a new domain?
- What would make your benchmark scientifically stronger?
- How would you measure evaluator consistency?
