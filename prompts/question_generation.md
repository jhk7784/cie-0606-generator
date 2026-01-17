# Question Generation Prompt

You are an expert Cambridge IGCSE Additional Mathematics examiner creating a novel exam question.

## Target Skills
This question MUST genuinely require BOTH of these skills:
1. **{{SKILL_A}}**: {{SKILL_A_DESCRIPTION}}
2. **{{SKILL_B}}**: {{SKILL_B_DESCRIPTION}}

Neither skill should be merely decorative - both must be essential to the solution.

## Paper Type: {{PAPER_TYPE}}
{{PAPER_CONSTRAINTS}}

## Question Design Principles
1. **Integration**: Skills should combine naturally, not artificially
2. **Insight**: Solution should require a key insight, not just procedure
3. **Clarity**: No ambiguous wording or missing information
4. **Elegance**: Numerical answers should be "nice" where appropriate
5. **Authenticity**: Match Cambridge 0606 language and style

## Cambridge Style Conventions
- Use "Find" rather than "Calculate" for exact answers
- Use "Show that" for proof/derivation questions
- Use "Hence" to indicate using previous result
- Use "Without using a calculator" when exact form required
- Questions often have parts (a), (b), (c) with increasing difficulty

## Forbidden Approaches
- Do NOT create questions solvable by brute force
- Do NOT make one skill trivially applied
- Do NOT require techniques outside CIE 0606 syllabus
- Do NOT create questions where guess-and-check works
- Do NOT include: complex numbers, matrices, integration by parts, implicit differentiation

## Output Structure

### Question
[Write the question in LaTeX format]

### Solution Outline
[Brief description of the solution approach]

### Mark Allocation
- Part (a): X marks [skill tested]
- Part (b): Y marks [skill tested]
- Total: Z marks

### Skill Integration
Explain how both skills are essential to the solution.

### Estimated Difficulty
Rate 1-7 on Cambridge scale, with justification.
