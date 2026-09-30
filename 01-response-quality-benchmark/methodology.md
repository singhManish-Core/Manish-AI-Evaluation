# Methodology

## 1. Study design

The benchmark uses a controlled prompt set. The same prompt is presented to two candidate responses, Response A and Response B.

Where multiple models are used, record the exact model/version and date. If model identity cannot be verified, label the source accurately instead of guessing.

## 2. Prompt design principles

Prompts should test different failure modes:

- straightforward factual questions
- multi-part instructions
- ambiguous wording
- technical explanation
- comparison
- reasoning
- translation/language quality
- edge cases
- requests requiring constraints
- questions where plausible-sounding misinformation is possible

Avoid prompts whose answer depends on obscure facts unless the verification method is documented.

## 3. Evaluation sequence

### Pass 1 — Independent scoring

Score A and B separately before deciding the pairwise winner.

### Pass 2 — Evidence check

For every score below 3 or above 4, write a short reason. For factual claims that materially affect the judgment, record a verification source.

### Pass 3 — Error taxonomy

Tag errors such as:

- Hallucination
- Factual error
- Unsupported claim
- Instruction failure
- Missing information
- Logical contradiction
- Overgeneralization
- Irrelevance
- Excessive verbosity
- Ambiguity not handled
- Technical misconception
- Calculation error
- Outdated information

### Pass 4 — Pairwise decision

Choose:

- A
- B
- Tie / effectively equivalent
- Neither / both materially deficient

Then provide a one- or two-sentence rationale.

## 4. Quality-control checks

Before finalizing an evaluation:

- Did I score the response against the rubric rather than personal preference?
- Did I separate factual correctness from writing style?
- Did I verify important factual claims?
- Did I penalize missing requested content?
- Did I avoid rewarding confident wording without evidence?
- Could another evaluator understand my reasoning?
- Did I apply the same standard to A and B?

## 5. Limitations

This is a portfolio study, not a scientific benchmark unless the final dataset, sampling protocol, evaluation process and statistical treatment support that claim.

Potential limitations include:

- limited prompt sample
- evaluator subjectivity
- model/version changes
- prompt sensitivity
- incomplete external verification
- single-evaluator bias
