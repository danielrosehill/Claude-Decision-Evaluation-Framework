# Decision Matrix Framework (Weighted Criteria)

## Framework Overview

**Purpose**: Evaluate a decision against multiple important criteria, with each criterion weighted by its relative importance to create an objective, quantified assessment.

**Best Used For**:
- Complex decisions with multiple factors
- Comparing options objectively
- Situations where trade-offs exist across different dimensions
- When personal biases need to be minimized
- Group decision-making (consistent evaluation method)

## Analysis Process

### Step 1: Define Evaluation Criteria

Identify 5-8 key criteria that matter for this decision.

**Common Criteria Categories**:
- **Financial**: Cost, ROI, budget impact
- **Time**: Time to implement, time saved, duration of benefit
- **Quality**: Expected outcomes, standards met
- **Risk**: Probability of failure, downside exposure
- **Strategic Fit**: Alignment with goals, long-term value
- **Feasibility**: Ease of implementation, resource availability
- **Impact**: Magnitude of change, number of people affected
- **Sustainability**: Long-term viability, maintenance requirements

**Criteria Guidelines**:
- Must be measurable or rateable
- Should be independent (not overlapping)
- Must be relevant to the specific decision
- Should cover different dimensions of the decision

### Step 2: Assign Weights to Each Criterion

Distribute 100 points across all criteria based on relative importance.

**Weighting Strategies**:
- **Equal weights**: 100 ÷ number of criteria (use when all factors matter equally)
- **Tiered weights**: Group into High (25-30%), Medium (15-20%), Low (5-10%)
- **Custom weights**: Reflect specific priorities for this decision

**Guidelines**:
- Most important criterion: typically 20-35%
- Least important criterion: typically 5-15%
- Total must equal exactly 100%

### Step 3: Rate the Decision on Each Criterion

For each criterion, assign a score from 0-10:

**Rating Scale**:
- 10: Exceptional/Excellent - far exceeds expectations
- 8-9: Very Good - exceeds expectations
- 6-7: Good - meets expectations
- 4-5: Fair - partially meets expectations
- 2-3: Poor - falls short of expectations
- 0-1: Very Poor - fails to meet expectations

**Rating Guidelines**:
- Be objective and evidence-based
- Use consistent standards across all criteria
- Consider both current state and projected outcomes
- Document reasoning for each score

### Step 4: Calculate Weighted Scores

For each criterion:
**Weighted Score** = (Criterion Rating ÷ 10) × Weight

**Example**:
- Criterion: "Financial Impact"
- Weight: 30%
- Rating: 7/10
- Weighted Score: (7 ÷ 10) × 30 = 21

### Step 5: Calculate Total Score

**Total Score** = Sum of all weighted scores

This will be a number from 0-100.

**Score Interpretation**:
- 85-100: Exceptional decision across criteria
- 70-84: Strong decision, well-aligned with priorities
- 55-69: Moderate decision, acceptable trade-offs
- 40-54: Weak decision, significant compromises
- Below 40: Poor decision, fails to meet key criteria

## Output Format

Your analysis MUST produce output in this exact format:

```markdown
## Decision Matrix Analysis Report

### Decision Being Evaluated
[Restate the decision clearly]

### Criteria and Weights

| Criterion | Weight (%) | Rationale for Weight |
|-----------|------------|---------------------|
| [Criterion 1] | [%] | [Why this weight] |
| [Criterion 2] | [%] | [Why this weight] |
| [Criterion 3] | [%] | [Why this weight] |
| ... | ... | ... |
| **Total** | **100%** | |

### Detailed Evaluation

#### Criterion 1: [Name] (Weight: [%])

**Rating**: [X]/10

**Rationale**: [Explain why this rating was assigned. What evidence supports it? What factors were considered?]

**Weighted Score**: [Calculated value]

---

#### Criterion 2: [Name] (Weight: [%])

**Rating**: [X]/10

**Rationale**: [Explain why this rating was assigned. What evidence supports it? What factors were considered?]

**Weighted Score**: [Calculated value]

---

[Repeat for all criteria]

### Scoring Summary

| Criterion | Weight | Raw Score | Weighted Score |
|-----------|--------|-----------|----------------|
| [Criterion 1] | [%] | [X]/10 | [Value] |
| [Criterion 2] | [%] | [X]/10 | [Value] |
| ... | ... | ... | ... |
| **TOTAL** | **100%** | — | **[Score]/100** |

### Score: [0-100]/100

### Performance Analysis

#### Strongest Criteria (Top 3)
1. **[Criterion]**: Scored [X]/10 - [Why it performed well]
2. **[Criterion]**: Scored [X]/10 - [Why it performed well]
3. **[Criterion]**: Scored [X]/10 - [Why it performed well]

#### Weakest Criteria (Bottom 3)
1. **[Criterion]**: Scored [X]/10 - [Why it underperformed]
2. **[Criterion]**: Scored [X]/10 - [Why it underperformed]
3. **[Criterion]**: Scored [X]/10 - [Why it underperformed]

### Interpretation

[2-3 paragraphs explaining:
- What the overall score indicates
- How the decision performs across weighted priorities
- Trade-offs revealed by the analysis
- Whether weak areas are acceptable given the strong areas]

### Key Insights

- **Critical Success Factor**: [Which high-weight criterion determines viability?]
- **Key Trade-off**: [What are you sacrificing and what are you gaining?]
- **Sensitivity Analysis**: [Which criterion, if it changed, would most impact the total score?]
- **Threshold Check**: [Does the decision meet minimum acceptable standards on must-have criteria?]

### Recommendation

Based on weighted criteria analysis: [Clear statement about whether the decision scores well enough to proceed]

### Scenario Analysis

**If priorities change**:
- If [Criterion X] becomes more important: [Impact on decision]
- If [Criterion Y] becomes less important: [Impact on decision]
```

## Analysis Guidelines

**Choose Relevant Criteria**: The criteria must actually matter for this specific decision. Don't use generic criteria if they don't apply.

**Honest Weighting**: Weights should reflect true priorities, not what sounds good. If cost really is 50% of the decision, weight it that way.

**Evidence-Based Ratings**: Each rating should be justified with specific reasons, not gut feelings.

**Consider Context**: A "7" in one criterion may represent different absolute levels than a "7" in another criterion. Be consistent within each criterion.

**Document Assumptions**: Note any assumptions made when rating, especially for future-oriented criteria.

**Identify Deal-breakers**: Some criteria may have minimum thresholds. Note if any criterion falls below an acceptable level, regardless of total score.

## Common Pitfalls to Avoid

- Using too many criteria (>10) - dilutes focus
- Making criteria overlap or double-count factors
- Assigning equal weights when priorities clearly differ
- Being influenced by one strong score when rating other criteria
- Ignoring absolute thresholds (some criteria may need minimum scores)
- Using vague criteria that can't be objectively rated
- Retrofitting weights to justify a predetermined conclusion
