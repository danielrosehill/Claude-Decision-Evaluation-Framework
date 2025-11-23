Analyze a decision from the queue using all seven decision-making frameworks in parallel.

**Instructions**:

1. Check for decision files in `/decisions/queue/`
2. If a specific decision filename is provided (e.g., `/analyze-decision career-change`), use that file. Otherwise, list available decisions and ask which to analyze.
3. Read the decision file completely
4. Launch 7 subagents IN PARALLEL (single message with 7 Task tool calls) with subagent_type='general-purpose', one for each framework:
   - Cost-Benefit Analysis
   - SWOT Analysis
   - Decision Matrix (Weighted Criteria)
   - ICE Framework
   - Risk-Reward Assessment
   - Eisenhower Matrix
   - Regret Minimization Framework
5. Each subagent should receive this prompt:

```
Analyze this decision using the [FRAMEWORK NAME] framework.

Decision file: [path to decision file]
Framework guide: /frameworks/[framework-file].md

Your task:
1. Read the decision file completely
2. Read the framework guide completely
3. Apply the framework to the decision following the guide EXACTLY
4. Use the precise output format specified in the framework guide
5. Be thorough, honest, and detailed in your analysis
6. Return the complete analysis report with score

The decision content is:
[paste full decision content here]
```

6. Wait for all 7 subagents to complete
7. Aggregate all results into a single comprehensive output file following the format specified in CLAUDE.md
8. Save the aggregated output to `/outputs/[YYYY-MM-DD-HHMM]-[decision-name].md`
9. Move the original decision file from `/decisions/queue/` to `/decisions/processed/`
10. Present the user with a summary dashboard showing all scores and key insights

**Important**:
- Use PARALLEL execution (single message with 7 Task calls)
- Keep framework analyses independent
- DO NOT create composite scores
- Follow the exact output format from CLAUDE.md
- Each framework report must be complete and detailed
