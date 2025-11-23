# Claude Decision Evaluation Framework - System Instructions

## Repository Purpose

This repository provides a structured system for analyzing major decisions through multiple objective frameworks. The goal is NOT to provide determinative answers, but to help users examine decisions from various analytical perspectives to make more informed choices.

## How This System Works

### Decision Input

Users place decision files in `/decisions/queue/`. Each decision file should be a markdown document describing:
- The decision to be made
- Context and background
- Options being considered
- Any constraints or requirements

### Analysis Process

When the `/analyze-decision` slash command is run:

1. **Read the decision** from `/decisions/queue/[filename]`
2. **Launch 7 parallel subagents** (using Task tool), one for each framework
3. **Each subagent**:
   - Reads its framework guide from `/frameworks/[framework-name].md`
   - Applies that framework to the decision
   - Produces a detailed analysis report with a 0-100 score
4. **Aggregate results** into a single combined output
5. **Save output** to `/outputs/[timestamp]-[decision-name].md`
6. **Move decision** from `/decisions/queue/` to `/decisions/processed/`

## The Seven Frameworks

Each framework is defined in `/frameworks/` with detailed instructions:

1. **cost-benefit-analysis.md** - Economic and practical viability analysis
2. **swot-analysis.md** - Strategic positioning (Strengths, Weaknesses, Opportunities, Threats)
3. **decision-matrix.md** - Multi-criteria weighted evaluation
4. **ice-framework.md** - Impact, Confidence, Ease scoring
5. **risk-reward-assessment.md** - Potential gains vs potential losses
6. **eisenhower-matrix.md** - Importance and urgency prioritization
7. **regret-minimization.md** - Long-term regret projection

## Critical Instructions for Analysis

### DO:
- **Run frameworks in parallel** using multiple Task tool calls in a single message
- **Keep frameworks independent** - each produces its own report and score
- **Use exact output format** specified in each framework guide
- **Be thorough and honest** in applying each framework
- **Preserve individual scores** - DO NOT create composite scores
- **Follow framework guidelines** exactly as written

### DO NOT:
- Create composite or average scores across frameworks
- Modify framework scoring methodologies
- Skip or abbreviate framework analysis
- Let one framework influence another
- Make recommendations that override framework outputs

## Subagent Prompts

When launching subagents for framework analysis, use prompts like:

```
Analyze the decision using the [Framework Name] framework.

1. Read the decision from [filepath]
2. Read the framework guide from /frameworks/[framework-name].md
3. Follow the framework guide EXACTLY - use the specified analysis process and output format
4. Apply the framework thoroughly and objectively
5. Return the complete analysis report with score

Be detailed, be honest, and follow the framework structure precisely.
```

## Output Aggregation Format

The combined output saved to `/outputs/` should be structured as:

```markdown
# Decision Analysis Run

**Decision**: [Name/title of decision]
**Analysis Date**: [ISO timestamp]
**Source File**: [Original decision file path]

---

## Decision Being Evaluated

[Full text of the decision from the input file]

---

## Framework Analysis Results

### 1. Cost-Benefit Analysis
**Score**: [X]/100

[Full report from framework]

---

### 2. SWOT Analysis
**Score**: [X]/100

[Full report from framework]

---

### 3. Decision Matrix (Weighted Criteria)
**Score**: [X]/100

[Full report from framework]

---

### 4. ICE Framework
**Score**: [X]/100

[Full report from framework]

---

### 5. Risk-Reward Assessment
**Score**: [X]/100

[Full report from framework]

---

### 6. Eisenhower Matrix
**Score**: [X]/100

[Full report from framework]

---

### 7. Regret Minimization Framework
**Score**: [X]/100

[Full report from framework]

---

## Summary Dashboard

| Framework | Score | Key Insight |
|-----------|-------|-------------|
| Cost-Benefit Analysis | [X]/100 | [1 sentence summary] |
| SWOT Analysis | [X]/100 | [1 sentence summary] |
| Decision Matrix | [X]/100 | [1 sentence summary] |
| ICE Framework | [X]/100 | [1 sentence summary] |
| Risk-Reward Assessment | [X]/100 | [1 sentence summary] |
| Eisenhower Matrix | [X]/100 | [1 sentence summary] |
| Regret Minimization | [X]/100 | [1 sentence summary] |

## Score Distribution

- Highest Score: [Framework name] ([Score]/100)
- Lowest Score: [Framework name] ([Score]/100)
- Score Range: [Highest - Lowest]
- Agreement Level: [High/Medium/Low based on standard deviation]

## Framework Consensus

**Frameworks supporting this decision** (score ≥ 60):
- [Framework name]: [score]
- [Framework name]: [score]

**Frameworks opposing this decision** (score < 40):
- [Framework name]: [score]
- [Framework name]: [score]

**Frameworks neutral** (score 40-60):
- [Framework name]: [score]

## User Guidance

This analysis is complete. Review each framework's detailed analysis to understand different perspectives on your decision. Pay special attention to:

1. Frameworks with extreme scores (very high or very low)
2. Areas of disagreement between frameworks
3. Insights that resonate most with your values
4. Factors you hadn't considered

**Remember**: This framework provides analysis, not answers. The final decision is yours, informed by these perspectives.
```

## File Naming Conventions

**Input files**: `/decisions/queue/[descriptive-name].md`

**Output files**: `/outputs/[YYYY-MM-DD-HHMM]-[decision-name].md`

**Processed decisions**: `/decisions/processed/[original-filename].md`

## Workflow Example

1. User creates `/decisions/queue/career-change.md`
2. User runs `/analyze-decision career-change`
3. Claude launches 7 parallel subagents
4. Each subagent analyzes using its framework
5. Claude aggregates results into `/outputs/2025-11-23-1430-career-change.md`
6. Claude moves `/decisions/queue/career-change.md` to `/decisions/processed/career-change.md`
7. User reviews the comprehensive analysis

## Best Practices

**For accuracy**: Follow framework guides precisely - they're designed to produce consistent, rigorous analysis.

**For speed**: Always use parallel Task tool calls (single message with multiple tool uses) when launching framework subagents.

**For quality**: Each framework should produce detailed, thoughtful analysis - not superficial checkbox responses.

**For usefulness**: The value is in seeing how different analytical lenses reveal different aspects of the decision.

## Error Handling

If a framework analysis fails:
- Note the failure in the output
- Continue with remaining frameworks
- Include partial results
- Explain what went wrong

## User Interaction

Be prepared to:
- Answer questions about specific framework scores
- Explain why frameworks disagreed
- Clarify framework methodologies
- Help users interpret results
- Suggest which frameworks might be most relevant for their specific decision type

## Philosophy

This system embodies the principle that **good decisions come from examining choices through multiple lenses**. No single framework is "right" - each illuminates different aspects. The user's job is to synthesize these perspectives with their own judgment, values, and context.
