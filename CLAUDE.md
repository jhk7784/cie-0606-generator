# CIE 0606 Additional Mathematics Question Generator

## Project Purpose
Automated generation of high-quality Cambridge IGCSE Additional Mathematics (0606)
exam questions using the MATH² methodology (Shah et al., 2024).

## Core Methodology
Questions are created by combining TWO skills from DIFFERENT topics.
This creates "out-of-distribution" problems that cannot be solved through
pattern matching alone.

---

## The 5-Stage Generation Pipeline

When asked to generate a question, ALWAYS follow these stages:

### Stage 1: Skill Selection
1. Read `skills/skill_taxonomy.json`
2. Select Skill A from one topic
3. Select Skill B from a DIFFERENT topic
4. Verify the pair can be meaningfully combined

### Stage 2: Question Generation
1. Read `prompts/question_generation.md`
2. Create a question that genuinely requires BOTH skills
3. Ensure neither skill is merely decorative
4. Design for insight, not just computation

### Stage 3: Solution Attempt
1. Attempt to solve the question yourself
2. Flag if calculations are excessive
3. Note any ambiguities or edge cases
4. Verify the answer is appropriate for the paper type

### Stage 4: Validation
1. Read `prompts/validation.md`
2. Check mathematical correctness
3. Verify all methods are within CIE 0606 syllabus
4. Confirm difficulty is appropriate (rate 1-7)

### Stage 5: CIE Formatting
1. Format question in LaTeX
2. Create mark scheme with M/A/B marks
3. Include step-by-step worked solution
4. Save to `output/questions/` and `output/markschemes/`

---

## CIE 0606 Syllabus Topics

| Topic | Content |
|-------|---------|
| 1 | Functions |
| 2 | Quadratic functions |
| 3 | Equations, inequalities and graphs |
| 4 | Indices and surds |
| 5 | Factors of polynomials |
| 6 | Simultaneous equations |
| 7 | Logarithmic and exponential functions |
| 8 | Straight line graphs |
| 9 | Circular measure |
| 10 | Trigonometry |
| 11 | Permutations and combinations |
| 12 | Series (Binomial & AP/GP) |
| 13 | Vectors in two dimensions |
| 14 | Differentiation and integration |

---

## Critical Constraints

### FORBIDDEN (Outside CIE 0606 Syllabus)
- Complex numbers
- Matrices
- 3D vectors
- Integration by parts
- Partial fractions
- Differential equations (beyond basic)
- Implicit differentiation
- Related rates (beyond basic)
- Maclaurin/Taylor series
- Proof by induction
- Statistics and probability distributions

### Paper-Specific Rules

**Paper 1 (2 hours, 80 marks)**
- Scientific calculator allowed
- 10-12 questions of varying length
- Questions increase in difficulty
- All topics may be examined

**Paper 2 (2 hours, 80 marks)**
- Scientific calculator allowed
- 10-12 questions of varying length
- Questions increase in difficulty
- All topics may be examined

### Answer Requirements
- Exact answers preferred where specified (fractions, surds, π)
- Decimal answers to 3 significant figures unless otherwise stated
- Angles in radians unless degrees specified

---

## Mark Scheme Conventions (Cambridge Style)

- **M1**: Method mark — correct approach shown
- **A1**: Accuracy mark — correct answer following correct method
- **B1**: Independent mark — awarded regardless of other marks
- **ft**: Follow through — mark subsequent work even with prior error
- **oe**: Or equivalent — accept equivalent forms
- **cao**: Correct answer only — no follow through
- **isw**: Ignore subsequent working
- **awrt**: Answer which rounds to

### Mark Allocation Guidelines
- 1-2 marks: Single step, routine calculation
- 3-4 marks: Two-step problem, moderate skill
- 5-7 marks: Multi-step, requires integration of concepts
- 8-12 marks: Extended problem, significant reasoning required

---

## File Locations

| Purpose | Location |
|---------|----------|
| Skill taxonomy | `skills/skill_taxonomy.json` |
| Generation prompt | `prompts/question_generation.md` |
| Validation prompt | `prompts/validation.md` |
| Skill extraction | `prompts/skill_extraction.md` |
| Framework reference | `docs/research_framework.md` |
| Generated questions | `output/questions/` |
| Mark schemes | `output/markschemes/` |
| Example questions | `seeds/` |

---

## Output Naming Convention

Questions: `output/questions/P{paper}_{topic1}-{topic2}_{skill1}-{skill2}_{date}.tex`
Mark schemes: `output/markschemes/MS_P{paper}_{topic1}-{topic2}_{skill1}-{skill2}_{date}.tex`

Example: `P1_T7-T14_LOG003-CALC008_20260117.tex`

---

## Quick Command Reference

When user says... → Do this:

"Generate a question" → Follow full 5-stage pipeline
"Random question" → Select random skills from different topics, then generate
"Validate this question" → Run through Stage 4 validation only
"Easier/harder" → Adjust skill complexity or mark allocation

---

## Key Formulae (Provided in Exam)

Students receive a formula sheet including:
- Quadratic formula
- Binomial theorem (positive integer n)
- Arithmetic and geometric series formulae
- Trigonometric identities (compound angles, double angles)
- Differentiation and integration standard results
- Arc length and sector area

When creating questions, remember students have access to these formulae.
