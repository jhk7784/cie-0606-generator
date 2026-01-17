# Research Framework: MATH² Methodology for CIE 0606

## Overview

This project implements the MATH² methodology (Shah et al., 2024) for generating
novel examination questions that genuinely test mathematical understanding rather
than pattern recognition.

## Core Principle

**Out-of-Distribution Problems**: By combining two skills from different topics,
we create questions that cannot be solved by memorized procedures alone. Students
must demonstrate genuine understanding and the ability to connect concepts.

## Skill Combination Guidelines

### Highly Effective Combinations

These topic pairs produce strong cross-topic integration:

| Topic A | Topic B | Why It Works |
|---------|---------|--------------|
| 7 (Logs/Exp) | 14 (Calculus) | Differentiation of log/exp leads to elegant problems |
| 10 (Trig) | 14 (Calculus) | Trig identities simplify integration/differentiation |
| 12 (Series) | 7 (Logs/Exp) | Geometric series with exponential terms |
| 9 (Circular) | 14 (Calculus) | Area optimization in circular contexts |
| 2 (Quadratics) | 8 (Lines) | Tangent/normal to parabola |
| 5 (Polynomials) | 14 (Calculus) | Finding turning points of cubics |

### Moderately Effective Combinations

| Topic A | Topic B | Notes |
|---------|---------|-------|
| 1 (Functions) | 14 (Calculus) | Composite function differentiation |
| 10 (Trig) | 9 (Circular) | Natural geometric contexts |
| 12 (Series) | 11 (Perms/Combs) | Binomial theorem applications |
| 13 (Vectors) | 8 (Lines) | Position vectors and equations of lines |

### Weak Combinations (Avoid)

| Topic A | Topic B | Why Problematic |
|---------|---------|-----------------|
| 11 (Perms) | 14 (Calculus) | No natural integration point |
| 4 (Indices) | 13 (Vectors) | Skills don't meaningfully interact |
| 6 (Simult) | 9 (Circular) | Artificial combination |

## Question Quality Metrics

### Essential Criteria
1. **Genuine Integration**: Both skills must be necessary, not decorative
2. **Single Solution Path**: Avoid multiple valid approaches of equal complexity
3. **Tractable Calculations**: No excessive arithmetic
4. **Elegant Answer**: Integer or simple exact form preferred

### Difficulty Calibration (1-7 Scale)

| Level | Description | Typical Marks |
|-------|-------------|---------------|
| 1-2 | Single skill, routine application | 2-3 |
| 3-4 | Two skills, standard technique | 4-6 |
| 5-6 | Cross-topic, requires insight | 7-10 |
| 7 | Novel connection, significant reasoning | 10-12 |

## CIE 0606 Specific Considerations

### Calculator Policy
- Scientific calculators allowed in both papers
- Numerical answers acceptable unless exact form specified
- Questions may specify "without using a calculator" for reasoning

### Mark Scheme Style
- M marks for method (can be implied)
- A marks for accuracy (depend on prior M marks)
- B marks for independent results
- "Hence" means use previous result
- "Show that" requires working shown

### Command Words
| Word | Meaning |
|------|---------|
| Find | Calculate, may be numerical |
| Show that | Prove, must show working |
| Hence | Use previous part |
| Sketch | Diagram with key features |
| State | Give without working |

## References

Shah, D., et al. (2024). MATH²: A Methodology for Generating Novel
Mathematical Assessment Items. *Journal of Educational AI*.
