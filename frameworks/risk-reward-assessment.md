# Risk-Reward Assessment Framework

## Framework Overview

**Purpose**: Evaluate decisions by systematically comparing potential gains (rewards) against potential losses (risks), weighted by the probability of each outcome.

**Best Used For**:
- High-stakes decisions
- Investment or financial decisions
- Situations with significant downside
- Ventures with uncertain outcomes
- When asymmetric risk/reward exists

## Analysis Process

### Step 1: Define Potential Outcomes

Identify the range of possible outcomes from best to worst.

**Best-Case Scenario** (maximum reward):
- What's the best realistic outcome?
- What would success look like?
- What are the upside possibilities?

**Worst-Case Scenario** (maximum risk):
- What's the worst realistic outcome?
- What could go wrong?
- What are the downside possibilities?

**Most Likely Scenario** (expected outcome):
- What's the probable outcome?
- What typically happens in similar situations?
- What's the "middle case"?

### Step 2: Quantify Rewards (Upside Potential)

Rate the best-case scenario: **0-10**

**Consider**:
- Magnitude of gain (financial, personal, strategic)
- Duration of benefit
- Compounding effects
- Life-changing potential
- Irreplaceable opportunities

**Rating Scale**:
- **10**: Life-changing, transformational reward
- **8-9**: Major, highly significant reward
- **6-7**: Substantial, meaningful reward
- **4-5**: Moderate, worthwhile reward
- **2-3**: Minor, incremental reward
- **0-1**: Negligible or trivial reward

**Be Specific**:
- Quantify in dollar terms if possible
- Identify non-financial rewards (time, relationships, growth)
- Consider second-order effects

### Step 3: Quantify Risks (Downside Exposure)

Rate the worst-case scenario: **0-10**

**Consider**:
- Magnitude of loss (financial, personal, strategic)
- Recoverability (can you bounce back?)
- Cascading effects
- Irreversible damage
- Worst-case realities

**Rating Scale**:
- **10**: Catastrophic, life-destroying risk
- **8-9**: Severe, major setback risk
- **6-7**: Significant, serious risk
- **4-5**: Moderate, manageable risk
- **2-3**: Minor, easily handled risk
- **0-1**: Negligible, trivial risk

**Types of Risk**:
- **Financial**: Money lost, debt incurred
- **Time**: Wasted time, delayed progress
- **Opportunity**: Better options foregone
- **Reputation**: Damaged credibility or relationships
- **Physical**: Health or safety concerns
- **Legal**: Regulatory or contractual exposure
- **Emotional**: Stress, regret, psychological cost

### Step 4: Assess Probabilities

Estimate the likelihood of each scenario.

**Probability of Success** (best or good outcome): **0-100%**

**Probability of Failure** (worst or bad outcome): **0-100%**

**Guidelines**:
- Base on evidence, data, or similar situations
- Account for your control over the outcome
- Consider external factors and dependencies
- Be realistic, not optimistic or pessimistic

**Reference Points**:
- 90%+: Near certain (strong evidence, proven approach)
- 70-89%: Highly likely (good evidence, favorable conditions)
- 50-69%: More likely than not (some evidence, mixed conditions)
- 30-49%: Less likely than not (limited evidence, challenges)
- 10-29%: Unlikely (weak evidence, significant barriers)
- <10%: Very unlikely (little evidence, major obstacles)

**Note**: Success and failure probabilities don't need to sum to 100% (there can be neutral outcomes).

### Step 5: Calculate Expected Value

**Expected Value** = (Reward × P(Success)) - (Risk × P(Failure))

This produces a score from -10 to +10.

**Normalize to 0-100 Scale**:
Final Score = 50 + (Expected Value × 5)

**Alternative Calculation** (if probabilities are uncertain):
Simple Risk-Reward Ratio = Reward ÷ Risk

### Step 6: Assess Risk-Reward Ratio

**Risk-Reward Ratio** = Potential Reward ÷ Potential Risk

**Interpretation**:
- **>3:1**: Highly favorable (reward much greater than risk)
- **2:1 to 3:1**: Favorable (reward clearly exceeds risk)
- **1:1 to 2:1**: Acceptable (reward somewhat exceeds risk)
- **0.5:1 to 1:1**: Marginal (risk and reward balanced or risk slightly higher)
- **<0.5:1**: Unfavorable (risk significantly exceeds reward)

### Step 7: Evaluate Risk Tolerance

**Context Questions**:
- Can you afford the worst-case outcome?
- Is this an asymmetric bet (limited downside, unlimited upside)?
- Does your situation favor risk-taking or risk-aversion?
- Are you "betting the farm" or making a calculated gamble?

## Output Format

Your analysis MUST produce output in this exact format:

```markdown
## Risk-Reward Assessment Report

### Decision Being Evaluated
[Restate the decision clearly]

### Scenario Analysis

#### Best-Case Scenario (Maximum Reward)
**Description**: [What happens if everything goes well]

**Potential Gains**:
- [Specific gain 1]
- [Specific gain 2]
- [Specific gain 3]

**Reward Rating**: [0-10]/10

**Reasoning**: [Why this rating? How significant are these gains?]

#### Worst-Case Scenario (Maximum Risk)
**Description**: [What happens if things go wrong]

**Potential Losses**:
- [Specific loss 1]
- [Specific loss 2]
- [Specific loss 3]

**Risk Rating**: [0-10]/10

**Reasoning**: [Why this rating? How severe are these losses?]

#### Most Likely Scenario (Expected Outcome)
**Description**: [What probably happens in reality]

**Expected Result**: [Realistic outcome]

### Probability Assessment

**Probability of Success**: [X]%

**Evidence Supporting This Probability**:
- [Data point or reasoning]
- [Data point or reasoning]
- [Data point or reasoning]

**Probability of Failure**: [Y]%

**Evidence Supporting This Probability**:
- [Data point or reasoning]
- [Data point or reasoning]
- [Data point or reasoning]

**Probability of Neutral/Mixed Outcome**: [Z]%

### Risk-Reward Metrics

**Potential Reward**: [Score]/10

**Potential Risk**: [Score]/10

**Risk-Reward Ratio**: [Ratio]:1

**Expected Value Calculation**:
- EV = (Reward × P(Success)) - (Risk × P(Failure))
- EV = ([Reward] × [P(Success)]) - ([Risk] × [P(Failure)])
- EV = [Result]

### Score: [0-100]/100

[Calculated as: 50 + (EV × 5)]

### Risk Analysis

#### Risk Factors
| Risk Type | Severity | Likelihood | Mitigable? | Mitigation Strategy |
|-----------|----------|------------|------------|---------------------|
| [Type] | [High/Med/Low] | [%] | [Yes/No/Partial] | [How to reduce] |
| [Type] | [High/Med/Low] | [%] | [Yes/No/Partial] | [How to reduce] |

#### Reward Factors
| Reward Type | Magnitude | Likelihood | Timeframe | Sustainability |
|-------------|-----------|------------|-----------|----------------|
| [Type] | [High/Med/Low] | [%] | [When] | [How long] |
| [Type] | [High/Med/Low] | [%] | [When] | [How long] |

### Interpretation

[2-3 paragraphs explaining:
- What the risk-reward profile indicates
- Whether the math supports taking this risk
- How probabilities affect the decision
- Key factors that could shift the assessment]

### Risk Tolerance Assessment

**Can you afford the worst case?**: [Yes/No/Partially]

**Explanation**: [Can you recover from maximum loss? What's at stake?]

**Asymmetry**: [Is this an asymmetric bet with limited downside and unlimited upside?]

**Position**: [Does your current situation favor risk-taking or risk-avoidance?]

### Key Insights

- **Biggest Risk**: [What's the primary downside concern?]
- **Biggest Reward**: [What's the primary upside opportunity?]
- **Key Uncertainty**: [What unknown factor most affects the outcome?]
- **Tipping Point**: [What would need to change to flip the decision?]

### Comparison to Benchmarks

**Versus doing nothing**: [How does the risk-reward compare to status quo?]

**Versus alternatives**: [How does this compare to other options?]

**Historical context**: [How does this compare to similar past decisions?]

### Recommendation

Based on risk-reward analysis: [Clear statement about whether the math justifies the risk]

**Risk Level**: [Low/Moderate/High/Extreme]

**Reward Potential**: [Low/Moderate/High/Exceptional]

**Overall Assessment**: [Is the reward worth the risk given probabilities?]
```

## Analysis Guidelines

**Separate Magnitude from Probability**: A severe risk with low probability may be acceptable. A small reward with low probability is not attractive.

**Be Realistic About Worst Cases**: Don't catastrophize, but don't be Pollyanna either. What's a genuinely bad but realistic outcome?

**Consider Recoverability**: A 10/10 risk that you can recover from in 6 months is different than one that permanently damages your life.

**Time Horizon Matters**: Short-term risks vs long-term rewards (or vice versa) affect the analysis.

**Account for Optionality**: Some decisions open future options (valuable) while others close them (costly).

**Quantify Where Possible**: Use actual numbers for financial risks and rewards, not just gut feelings.

## Common Pitfalls to Avoid

- Focusing only on upside while ignoring downside
- Underestimating the probability of failure (optimism bias)
- Failing to consider cascading or second-order risks
- Ignoring non-financial risks (reputation, time, relationships)
- Not stress-testing your probability estimates
- Confusing acceptable risk with favorable risk-reward
- Treating all risks as equal when some are existential and others are manageable
