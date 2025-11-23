# Cost-Benefit Analysis Framework

## Framework Overview

**Purpose**: Quantify and compare the costs and benefits of a decision to determine its economic and practical viability.

**Best Used For**:
- Financial decisions
- Resource allocation
- Investment choices
- Major purchases or commitments
- Time-intensive projects

## Analysis Process

### Step 1: Identify All Costs

List every cost associated with this decision, including:

**Direct Costs**:
- Monetary expenses (initial and ongoing)
- Time investment (hours/days/months)
- Resources required (equipment, space, materials)

**Indirect Costs**:
- Opportunity costs (what you're giving up)
- Maintenance and upkeep
- Training or learning curve
- Potential risks and liabilities

**Intangible Costs**:
- Stress and emotional burden
- Relationship impacts
- Lifestyle changes
- Reputation or social costs

### Step 2: Identify All Benefits

List every benefit from this decision, including:

**Direct Benefits**:
- Financial gains (immediate and projected)
- Time saved or efficiency gained
- Tangible assets acquired
- Skills or knowledge gained

**Indirect Benefits**:
- Strategic advantages
- Network expansion
- Future opportunities unlocked
- Competitive positioning

**Intangible Benefits**:
- Personal satisfaction
- Quality of life improvements
- Peace of mind
- Alignment with values

### Step 3: Quantify Costs and Benefits

For each cost and benefit:
1. Assign a monetary value where possible
2. If not monetary, assign a point value (1-10 scale)
3. Consider time horizons (short-term vs long-term)
4. Account for probability (multiply by likelihood %)

### Step 4: Calculate Metrics

**Total Costs** = Sum of all cost values

**Total Benefits** = Sum of all benefit values

**Net Benefit** = Total Benefits - Total Costs

**Benefit-Cost Ratio** = Total Benefits ÷ Total Costs

**Return on Investment (ROI)** = (Net Benefit ÷ Total Costs) × 100%

### Step 5: Scoring

Convert analysis to a 0-100 score:

**Scoring Formula**:
- If Net Benefit ≥ 0: Score = min(100, 50 + (ROI/2))
- If Net Benefit < 0: Score = max(0, 50 + (ROI/2))

**Score Interpretation**:
- 80-100: Highly favorable economics
- 60-79: Favorable, clear positive return
- 40-59: Marginally positive or break-even
- 20-39: Marginally negative
- 0-19: Strongly unfavorable economics

## Output Format

Your analysis MUST produce output in this exact format:

```markdown
## Cost-Benefit Analysis Report

### Decision Being Evaluated
[Restate the decision clearly]

### Cost Analysis

#### Direct Costs
- [Item]: [Value/Points] - [Explanation]
- [Item]: [Value/Points] - [Explanation]

#### Indirect Costs
- [Item]: [Value/Points] - [Explanation]
- [Item]: [Value/Points] - [Explanation]

#### Intangible Costs
- [Item]: [Value/Points] - [Explanation]

**Total Costs**: [Value]

### Benefit Analysis

#### Direct Benefits
- [Item]: [Value/Points] - [Explanation]
- [Item]: [Value/Points] - [Explanation]

#### Indirect Benefits
- [Item]: [Value/Points] - [Explanation]
- [Item]: [Value/Points] - [Explanation]

#### Intangible Benefits
- [Item]: [Value/Points] - [Explanation]

**Total Benefits**: [Value]

### Financial Metrics

- **Net Benefit**: [Value]
- **Benefit-Cost Ratio**: [Ratio]:1
- **Return on Investment**: [%]

### Score: [0-100]/100

### Interpretation

[2-3 paragraphs explaining:
- What the numbers tell us
- Key trade-offs identified
- Economic viability
- Factors that could shift the analysis]

### Key Insights

- **Biggest Cost Factor**: [What and why]
- **Biggest Benefit Factor**: [What and why]
- **Critical Assumption**: [What assumption is this analysis most dependent on?]
- **Breakeven Point**: [What would need to change for this to be worthwhile/not worthwhile?]

### Recommendation

Based purely on cost-benefit economics: [Clear statement about whether the numbers support this decision]
```

## Analysis Guidelines

**Be Thorough**: Don't skip categories. If a category doesn't apply, state "N/A" with brief explanation.

**Be Realistic**: Use conservative estimates. It's better to underestimate benefits and overestimate costs.

**Show Your Work**: Explain how you arrived at quantifications, especially for intangibles.

**Time Value**: Consider when costs and benefits occur. A benefit in 5 years is worth less than a benefit today.

**Probability Weighting**: If a benefit or cost is uncertain, multiply by probability of occurrence.

**Context Matters**: A $1000 cost means different things to different people in different situations.

## Common Pitfalls to Avoid

- Ignoring opportunity costs
- Failing to account for time value of money
- Overlooking hidden or future costs
- Being overly optimistic about benefits
- Not considering the full time horizon
- Treating sunk costs as relevant
- Ignoring intangible factors entirely
