# Claude Decision Evaluation Framework

A structured system for analyzing major life and business decisions through multiple objective frameworks using Claude Code.

## Purpose

This framework helps you examine important decisions from seven different analytical perspectives. It's **not** designed to tell you what to do, but rather to:

- Illuminate different aspects of your decision
- Reveal trade-offs and considerations you might have missed
- Provide objective scoring across multiple dimensions
- Help you think more clearly about complex choices

## How It Works

### 1. Write Your Decision

Create a markdown file in `/decisions/queue/` describing your decision:

```markdown
# Should I Accept the Job Offer?

## Context
I've been offered a senior engineering role at a startup...

## Current Situation
I currently work at a stable corporation with...

## The Options
1. Accept the startup offer
2. Stay at current company
3. Negotiate for different terms

## Constraints
- Need to decide within 2 weeks
- Family considerations...
```

### 2. Run the Analysis

In Claude Code, run:

```bash
/analyze-decision your-decision-name
```

Claude will analyze your decision through **seven frameworks simultaneously**:

1. **Cost-Benefit Analysis** - Economic viability and practical value
2. **SWOT Analysis** - Strategic positioning and competitive factors
3. **Decision Matrix** - Multi-criteria weighted evaluation
4. **ICE Framework** - Impact, Confidence, and Ease scoring
5. **Risk-Reward Assessment** - Potential gains vs potential losses
6. **Eisenhower Matrix** - Importance and urgency prioritization
7. **Regret Minimization** - Long-term perspective and future regret

### 3. Review the Results

Each framework produces:
- A detailed analysis report
- An objective 0-100 score
- Key insights and recommendations

You'll receive a comprehensive output showing:
- All seven framework reports
- Individual scores (NOT averaged)
- Areas of agreement and disagreement
- Summary dashboard

## The Seven Frameworks

### 1. Cost-Benefit Analysis
**Best for**: Financial decisions, resource allocation, investments

Quantifies all costs (financial, time, opportunity) against all benefits to calculate net value and ROI.

**Score Interpretation**:
- 80-100: Highly favorable economics
- 60-79: Clear positive return
- 40-59: Break-even or marginal
- 20-39: Marginally negative
- 0-19: Strongly unfavorable

### 2. SWOT Analysis
**Best for**: Strategic decisions, career moves, competitive situations

Examines Strengths, Weaknesses, Opportunities, and Threats to determine strategic positioning.

**Score Interpretation**:
- 80-100: Very strong strategic position
- 60-79: Favorable position
- 40-59: Balanced, depends on execution
- 20-39: Challenging position
- 0-19: Very weak position

### 3. Decision Matrix (Weighted Criteria)
**Best for**: Complex multi-factor decisions, comparing options objectively

Evaluates the decision against 5-8 key criteria, each weighted by importance.

**Score Interpretation**:
- 85-100: Exceptional across criteria
- 70-84: Strong decision
- 55-69: Moderate, acceptable trade-offs
- 40-54: Weak, significant compromises
- Below 40: Fails to meet key criteria

### 4. ICE Framework
**Best for**: Prioritization, resource-constrained choices, quick wins

Scores based on Impact (how significant), Confidence (how certain), and Ease (how simple).

**Score Interpretation**:
- 80-100: Exceptional opportunity
- 60-79: Strong opportunity
- 40-59: Moderate opportunity
- 20-39: Weak opportunity
- 0-19: Poor opportunity

### 5. Risk-Reward Assessment
**Best for**: High-stakes decisions, uncertain outcomes, asymmetric bets

Compares best-case rewards against worst-case risks, weighted by probability.

**Score Interpretation**:
- 70-100: Reward clearly exceeds risk
- 50-69: Favorable risk-reward ratio
- 30-49: Balanced or slightly risky
- 10-29: Risk exceeds reward
- 0-9: Unfavorable risk exposure

### 6. Eisenhower Matrix
**Best for**: Time management, prioritization, distinguishing urgent from important

Classifies decisions by Importance (goal alignment) and Urgency (time sensitivity).

**Score Interpretation**:
- 85-100: Urgent & Important (Do First)
- 65-84: Important, Not Urgent (Schedule)
- 35-64: Urgent, Not Important (Delegate)
- 0-34: Neither (Eliminate)

### 7. Regret Minimization Framework
**Best for**: Life-changing decisions, values-based choices, risk vs safety

Projects future regret at 1, 5, and 10+ years, asking which choice you'd regret least.

**Score Interpretation**:
- 70-100: Low regret if you DO this
- 55-69: Moderate preference for doing
- 45-54: Similar regret either way
- 30-44: Moderate preference for NOT doing
- 0-29: Low regret if you DON'T do this

## Repository Structure

```
Claude-Decision-Evaluation-Framework/
├── decisions/
│   ├── queue/              # Place new decisions here
│   └── processed/          # Analyzed decisions move here
├── frameworks/             # Framework methodology guides
│   ├── cost-benefit-analysis.md
│   ├── swot-analysis.md
│   ├── decision-matrix.md
│   ├── ice-framework.md
│   ├── risk-reward-assessment.md
│   ├── eisenhower-matrix.md
│   └── regret-minimization.md
├── outputs/                # Analysis results saved here
├── templates/              # Decision templates
├── .claude/
│   └── commands/
│       └── analyze-decision.md  # The slash command
├── CLAUDE.md              # Instructions for Claude
└── README.md              # This file
```

## Getting Started

### 1. Set Up

Clone this repository and open it in Claude Code:

```bash
git clone <repository-url>
cd Claude-Decision-Evaluation-Framework
claude-code
```

### 2. Create Your First Decision

Use the template in `/templates/decision-template.md` to create your decision file in `/decisions/queue/`.

### 3. Run Analysis

```bash
/analyze-decision
```

Claude will list available decisions if you don't specify a filename.

### 4. Review Results

Check `/outputs/` for your comprehensive analysis report.

## Example Use Cases

**Career Decisions**:
- Job offers
- Career changes
- Freelancing vs employment
- Starting a business

**Financial Decisions**:
- Major purchases
- Investments
- Relocations
- Education/training

**Personal Decisions**:
- Relationships
- Lifestyle changes
- Health commitments
- Long-term goals

**Business Decisions**:
- Product launches
- Strategic pivots
- Hiring decisions
- Partnership opportunities

## Interpreting Results

### When Frameworks Agree (High Consensus)
Multiple frameworks scoring similarly indicates:
- Clear-cut decision
- Consistent factors across dimensions
- Higher confidence in the direction

### When Frameworks Disagree (Low Consensus)
Frameworks with divergent scores indicate:
- Complex trade-offs
- Different priorities matter
- Need for deeper reflection on values
- Context-dependent decision

### Pay Special Attention To:
1. **Extreme scores** (very high or very low) - these reveal strong signals
2. **Regret Minimization** - often provides the clearest long-term perspective
3. **Risk-Reward** - critical for understanding downside exposure
4. **Your gut reaction** - which frameworks resonate with your intuition?

## Best Practices

**Be Honest**: The frameworks only work if you're truthful about your situation, constraints, and feelings.

**Provide Context**: More detail in your decision description leads to better analysis.

**Don't Cherry-Pick**: Review ALL framework results, even ones that disagree with your preference.

**It's a Tool, Not a Dictator**: These frameworks inform your decision; they don't make it for you.

**Revisit Over Time**: Some decisions benefit from running the analysis multiple times as circumstances change.

## Limitations

This framework has important limitations:

- **Not deterministic**: It won't tell you definitively what to do
- **Garbage in, garbage out**: Analysis quality depends on input quality
- **No moral judgments**: Frameworks are amoral - they don't evaluate ethics
- **Context-blind**: AI doesn't know your full life context
- **Quantification limits**: Not everything can be scored numerically
- **No guarantee**: Following framework recommendations doesn't guarantee success

## Philosophy

Good decisions come from examining choices through multiple lenses. Each framework reveals different aspects:

- **Cost-Benefit** focuses on efficiency and value
- **SWOT** focuses on strategic positioning
- **Decision Matrix** focuses on prioritized criteria
- **ICE** focuses on achievability and impact
- **Risk-Reward** focuses on asymmetry and probabilities
- **Eisenhower** focuses on time and importance
- **Regret Minimization** focuses on long-term perspective

Your job is to synthesize these perspectives with your own judgment, values, and context to make the best decision for YOU.

## Customization

You can customize this framework:

- Modify framework guides in `/frameworks/` to adjust methodologies
- Create new frameworks following the same pattern
- Adjust scoring scales to suit your preferences
- Add custom criteria to Decision Matrix

## Contributing

Improvements welcome:
- Better framework methodologies
- Additional frameworks
- Template improvements
- Documentation enhancements

## License

[Specify your license]

## Credits

Built for use with [Claude Code](https://www.anthropic.com/claude/code) by Anthropic.

Framework methodologies adapted from established decision-making systems:
- Cost-Benefit Analysis (Economics)
- SWOT Analysis (Business Strategy)
- Decision Matrix (Decision Science)
- ICE Framework (Growth Hacking)
- Risk-Reward Assessment (Finance)
- Eisenhower Matrix (Productivity)
- Regret Minimization (Behavioral Economics)
