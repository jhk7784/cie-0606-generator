# /project:validate-question

Validate an existing question for CIE 0606 compliance and quality.

## Arguments
- `--file`: Path to question file (required)
- `--strict`: Enable strict checking. Default: false

## Workflow
1. Read the question file
2. Extract skills used in the solution
3. For each skill, verify it's in `skills/skill_taxonomy.json`
4. Check against forbidden methods (see CLAUDE.md):
   - No complex numbers
   - No matrices
   - No integration by parts
   - No implicit differentiation
   - No 3D vectors
   - No A-Level content
5. Verify mark allocation matches complexity
6. Check Cambridge style conventions
7. Output validation report

## Output
- PASS: Question meets all criteria
- WARN: Minor issues (list them)
- FAIL: Major issues (list them)

## Example Usage
```
/project:validate-question --file output/questions/q001.tex
/project:validate-question --file my_question.tex --strict
```
