# Data Analysis Truth

*Numbers lie when you let them.*

## The Prompt

For every analysis, answer these before you start:

1. **What question will this answer?** (One sentence)
2. **What would prove you wrong?**
3. **What are you hoping to find?** (Bias check)
4. **Who needs to believe this?**

Apply clarity principles:

- **Lead with the conclusion** - Don't make stakeholders hunt for insights
- **Use plain language** - "Users drop off" not "conversion rates demonstrate suboptimal performance"
- **Show, don't tell** - One clear chart beats three paragraphs
- **Address the objection** - Why might this data mislead?

## A/B Testing Design

When you need to test solutions, not just analyze existing data:

### Experiment Planning
**Before running any test:**
1. **Hypothesis**: "We believe that [change] will result in [outcome] because [reasoning]"
2. **Success metric**: Primary KPI that defines winning variant
3. **Sample size**: Calculate statistical power needed for detection
4. **Test duration**: Balance statistical significance with business timeline

### Test Design Principles
**Control variables:**
- Change one thing at a time
- Maintain consistent user experience within variants
- Account for seasonality and external factors
- Plan for segment-specific analysis (new vs. returning users)

**Measurement discipline:**
- **Primary metric**: Single most important success indicator
- **Secondary metrics**: Supporting indicators and guardrails
- **Guardrail metrics**: What must not get worse (revenue, retention)
- **Leading indicators**: Early signals before primary metric moves

### Statistical Rigor
**Avoid common mistakes:**
- **Peeking**: Don't stop test early because you see results
- **P-hacking**: Don't hunt for significant segments post-hoc
- **HARKing**: Don't hypothesize after results are known
- **Simpson's paradox**: Check for segment-level reversals

**Sample size calculation:**
- Baseline conversion rate
- Minimum detectable effect (practical significance)
- Statistical power (typically 80%)
- Significance level (typically 5%)

### Results Interpretation
**Statistical significance vs. practical significance:**
- A 0.1% improvement might be statistically significant but not worth implementing
- Consider effort required vs. business impact
- Factor in long-term maintenance costs

**Common interpretation errors:**
- Assuming no effect when test is underpowered
- Confusing correlation with causation
- Ignoring confidence intervals for effect size
- Not considering user segment differences

## The Reality

Perfect data doesn't exist. Good decisions do. A/B testing gives you confidence, not certainty.

## Practice

Explain your key finding in one sentence. If you can't, you haven't found it yet. For experiments, can you explain why the winning variant worked?