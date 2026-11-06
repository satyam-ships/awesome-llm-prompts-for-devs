# awesome-llm-prompts-for-devs 💬

> Copy-paste prompt templates for everyday engineering work. Fill in the `{{placeholders}}`.

## Principles
Give context · state the output format · include constraints · ask for reasoning on hard problems · paste the real error, not a paraphrase.

## Code review
```
Review this diff for correctness bugs, security issues and missing tests.
For each issue: file:line, what breaks, a triggering input, a fix.
Skip style nits. Diff:
{{diff}}
```

## Debugging
```
Error: {{full error and stack trace}}
Code: {{relevant snippet}}
What I expected: {{expected}}  What happened: {{actual}}
List 3 likely root causes ranked by probability and the cheapest check for each.
```

## Write tests
```
Write {{framework}} tests for this function. Cover happy path, empty/null, boundaries,
and error paths. Don't mock internals. Function:
{{code}}
```

## Refactor safely
```
Refactor for readability without changing behavior. Keep public signatures.
Explain each change in one line and flag any behavior risk. Code:
{{code}}
```

## Explain unfamiliar code
```
Explain this code to a developer new to {{language}}: purpose, data flow, and any gotchas. Code:
{{code}}
```

## Design review
```
Here is my design: {{design}}. Scale: {{scale}}. Identify the top 3 failure modes,
bottlenecks, and what I should measure before building.
```

## SQL optimization
```
Schema: {{ddl}}
Slow query: {{sql}}
EXPLAIN output: {{plan}}
Suggest index or rewrite changes and explain the expected plan difference.
```

## Commit messages
```
Write a Conventional Commit message for this diff. Subject <= 72 chars, body explains why. Diff:
{{diff}}
```

See also: [awesome-coding-agent-skills](../awesome-coding-agent-skills). License: [MIT](LICENSE).
