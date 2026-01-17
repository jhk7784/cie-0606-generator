# Skill Extraction Prompt

You are analyzing a CIE 0606 Additional Mathematics exam question to extract the atomic mathematical skills it tests.

## Input Question
{{QUESTION_TEXT}}

## Instructions
1. Identify ALL mathematical skills required to solve this question
2. For each skill, provide:
   - Skill ID (format: TOPIC-XXX)
   - Skill name (brief, specific)
   - Topic number (1-14)
   - Whether it's primary or secondary

## Output Format
```json
{
  "skills": [
    {
      "id": "CALC-005",
      "name": "Chain rule",
      "topic": 14,
      "role": "primary"
    },
    {
      "id": "TRIG-006",
      "name": "Compound angle formulae",
      "topic": 10,
      "role": "secondary"
    }
  ],
  "difficulty": 5,
  "paper_type": 1
}
```

## CIE 0606 Topics Reference
1. Functions
2. Quadratic functions
3. Equations, inequalities and graphs
4. Indices and surds
5. Factors of polynomials
6. Simultaneous equations
7. Logarithmic and exponential functions
8. Straight line graphs
9. Circular measure
10. Trigonometry
11. Permutations and combinations
12. Series
13. Vectors in two dimensions
14. Differentiation and integration
