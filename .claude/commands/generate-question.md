# /project:generate-question

Generate a novel CIE 0606 Additional Mathematics question using the 5-stage MATH² pipeline.

## Arguments
- `--paper`: Paper type (1 or 2). Default: 1
- `--skill-a`: First skill ID. Default: random
- `--skill-b`: Second skill ID. Default: random
- `--difficulty`: Target difficulty 1-7. Default: 4
- `--topic`: Primary topic focus (1-14). Default: any

## Workflow

### Stage 1: Skill Selection
1. Load `skills/skill_taxonomy.json`
2. If skills not specified, randomly select from different topics
3. Verify pair compatibility

### Stage 2: Question Generation
1. Load `prompts/question_generation.md`
2. Fill in skill details
3. Generate question requiring both skills genuinely

### Stage 3: Solution Attempt
1. Solve the question step-by-step
2. Check for computational tractability
3. Verify answer is appropriate

### Stage 4: Validation
1. Load `prompts/validation.md`
2. Check mathematical correctness
3. Verify CIE 0606 syllabus compliance
4. Rate difficulty 1-7

### Stage 5: Output
1. Format as Cambridge-style question (LaTeX)
2. Create mark scheme with M/A/B marks
3. Save question to `output/questions/`
4. Save mark scheme to `output/markschemes/`
5. Report what was generated

## Example Usage
```
/project:generate-question
/project:generate-question --paper 1 --difficulty 5
/project:generate-question --skill-a LOG-003 --skill-b CALC-008
/project:generate-question --topic 14
```
