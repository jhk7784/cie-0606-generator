# /project:batch-generate

Generate multiple CIE 0606 questions in batch.

## Arguments
- `--count`: Number of questions. Default: 5
- `--paper`: Restrict to paper type (1 or 2). Default: any
- `--topic`: Focus on topic (1-14). Default: any
- `--difficulty`: Target difficulty 1-7. Default: 4

## Workflow
1. For each question (1 to count):
   a. Select random skill pair from different topics
   b. Run /project:generate-question
   c. Log success/failure
   d. If failed, retry with different pair (max 3 retries)
2. Save summary report to `output/batch_report_{date}.md`
3. List all generated files

## Example Usage
```
/project:batch-generate --count 10
/project:batch-generate --count 5 --paper 1
/project:batch-generate --count 20 --topic 14
/project:batch-generate --count 10 --difficulty 6
```
