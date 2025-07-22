# Prioritization Methods Framework

*Cut through opinion with systematic scoring*

## The Prompt

Stop arguing about priorities. Use proven frameworks to make objective, defendable decisions about what to build next.

## Method Selection Guide

**Choose your framework based on context:**

### RICE Framework
**Best for:** Feature prioritization with cross-functional teams
- **Reach**: How many users affected (number per quarter)
- **Impact**: Improvement per user (1-3 scale: minimal/low/medium/high/massive)
- **Confidence**: How sure are you (% as decimal: 0.5-1.0)  
- **Effort**: Team-months required (engineering estimate)

**Score = (Reach × Impact × Confidence) ÷ Effort**

### ICE Framework  
**Best for:** Quick prioritization when data is limited
- **Impact**: Business value (1-10 scale)
- **Confidence**: How certain you are (1-10 scale)
- **Ease**: How easy to implement (1-10 scale, 10 = easiest)

**Score = (Impact + Confidence + Ease) ÷ 3**

### Kano Model
**Best for:** Understanding user satisfaction vs. feature investment
- **Basic**: Must-have features (prevent dissatisfaction)
- **Performance**: Linear satisfaction improvement
- **Excitement**: Delight features that differentiate
- **Indifferent**: Features users don't care about
- **Reverse**: Features that actually hurt satisfaction

### Value vs. Effort Matrix
**Best for:** Portfolio view and resource allocation
- Plot initiatives on 2x2 grid: High/Low Value × High/Low Effort
- **Quick wins**: High value, low effort (do first)
- **Major projects**: High value, high effort (plan carefully)
- **Fill-ins**: Low value, low effort (do if capacity)
- **Money pits**: Low value, high effort (avoid)

## Framework Application

### Step 1: Data Collection
**For RICE/ICE scoring:**
- User analytics for reach estimates
- A/B test results for impact data
- Engineering estimates for effort
- Customer feedback for confidence levels

### Step 2: Scoring Discipline
**Scoring guidelines:**
- Use same team for consistency
- Document scoring rationale
- Update scores with new data
- Review scores quarterly

### Step 3: Decision Making
**Priority thresholds:**
- RICE score >10: Strong candidate
- ICE score >7: Consider for roadmap
- Always consider strategic fit alongside scores

## Advanced Techniques

### Weighted Scoring
**When business priorities aren't equal:**
- Assign weights to different business objectives
- Multiply initiative scores by relevant weights
- Useful for balancing growth vs. retention vs. technical debt

### Opportunity Solution Tree
**For complex problem spaces:**
- Map user problems to business outcomes
- Generate multiple solution options per problem
- Score solutions within problem context
- Maintains user focus while enabling comparison

### Buy a Feature
**For stakeholder alignment:**
- Give stakeholders "budget" to "buy" features
- Forces difficult trade-off conversations
- Reveals true preferences vs. stated priorities
- Useful for enterprise customer input

## Common Pitfalls

- **Scoring inflation**: Everyone rates their ideas as high impact
- **False precision**: Don't over-engineer with complex formulas
- **Ignoring strategic fit**: High scores don't override strategy
- **Static scoring**: Update scores as you learn
- **Analysis paralysis**: Use framework to decide, not postpone

## The Reality

**Perfect prioritization doesn't exist.** Good prioritization:
- Makes trade-offs explicit
- Can be explained to stakeholders
- Updates based on new information
- Balances data with strategy

## Quick Decision Framework

**When you need to prioritize fast:**
1. What's the user problem?
2. How many users have this problem?
3. How confident are we this solution works?
4. How much effort to build and maintain?
5. Does this advance our strategy?

Three "yes" answers = strong candidate.

## Practice

Take your current backlog. Score top 10 items with RICE. Rank by score. Compare to your gut instinct ranking. Investigate large differences - either data is wrong or intuition needs updating.