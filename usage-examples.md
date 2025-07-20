# Claude Code Usage Examples

*PM scenarios using this library*

## Scenario 1: Strategy Document Review

**Situation**: Need to review a team's Q4 strategy document

```
/strategy-review strategy-q4.md

Claude applies the good-strategy-framework, flags:
- Vague problem diagnosis ("need to improve user experience")  
- Goals masquerading as strategy ("increase engagement 15%")
- Incoherent action list without connecting logic

Output: Specific rewrite suggestions using Rumelt's kernel
```

## Scenario 2: Feature Specification Creation

**Situation**: Engineering needs a clear PRD for new onboarding flow

```
/feature-spec "improve user onboarding"

Claude structures:
- Problem: New users abandon setup because current flow has 7 steps
- Solution: Build 3-step guided onboarding with progress indicators  
- Success: 80% setup completion (vs current 45%)
- Trade-off: Won't build advanced customization to ship faster
```

## Scenario 3: Stakeholder Alignment

**Situation**: Need buy-in from legal team for data collection feature

```
/stakeholder-sync "get legal approval for user analytics"

Claude creates:
- Clear ask: "Need legal review of user event tracking by Friday"
- Context: Specific data types and usage
- Dependencies: "Need your sign-off to proceed with engineering"
- Next steps: "I'll schedule 30min review Thursday if questions"
```

## Scenario 4: Research Planning

**Situation**: Understanding why enterprise customers churn

```
/research-plan "enterprise churn research"

Claude forces clarity:
- Decision this informs: Should we build admin dashboards or improve onboarding?
- What would change mind: If customers leave due to pricing not features
- Research question: "Why did you stop using our tool?" (not leading)
- Bias check: Are we assuming it's a feature problem?
```

## Integration Power

These commands work together: strategy informs features, features need stakeholder buy-in, buy-in requires research insights. The library supports systematic PM workflows.