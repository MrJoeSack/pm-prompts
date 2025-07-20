# Strategy Check Command Test

## Test Input 1: Product Strategy Document
```
/strategy-check
Strategy: "We will leverage best-in-class technology to deliver world-class user experiences and achieve market leadership through innovative solutions that drive customer success."
Context: B2B SaaS product, competitive market
Resources: 20-person team, 18-month timeline
```

## Expected Output Validation:
- [ ] Identifies bad strategy warning signs (fluff language)
- [ ] Points out missing diagnosis of specific challenge
- [ ] Flags goals masquerading as strategy
- [ ] Suggests specific improvements using Rumelt's framework
- [ ] Requires coherent action identification
- [ ] Tests for three-sentence clarity

## Test Input 2: Go-to-Market Strategy
```
/strategy-check
Strategy: "Increase market share by 25% through enhanced sales enablement, improved product positioning, and strategic partnerships while maintaining customer satisfaction above 90%."
Context: Established product entering new vertical
Timeline: 12 months
```

## Expected Output Validation:
- [ ] Distinguishes between goals and strategy
- [ ] Identifies missing guiding policy
- [ ] Checks for coherent action coordination
- [ ] Assesses resource allocation logic
- [ ] Tests for specific challenge diagnosis
- [ ] Validates strategic coherence

## Test Input 3: Feature Strategy
```
/strategy-check
Strategy: "Build comprehensive mobile app with native iOS and Android versions, web portal integration, offline functionality, push notifications, and advanced analytics to compete with market leaders."
Context: Currently web-only product
Resources: 8 engineers, 6-month deadline
```

## Expected Output Validation:
- [ ] Flags scope vs. resource mismatch
- [ ] Identifies lack of guiding policy
- [ ] Points out action list without coherence
- [ ] Suggests focus and prioritization
- [ ] Tests against resource constraints
- [ ] Requires specific challenge identification