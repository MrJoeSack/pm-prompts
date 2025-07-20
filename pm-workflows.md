# PM Workflow Guide

*How product managers actually use this library day-to-day*

## Daily PM Scenarios

**Morning Email Triage**
- Copy unclear stakeholder email → Apply stakeholder-communication framework → Draft clear response
- Pattern: "Use the stakeholder-communication prompt to help me respond to this request"

**Document Review**
- Download strategy doc → `/strategy-review filename.txt` → Flag issues before team meeting
- Pattern: Apply frameworks before sending to stakeholders

**Feature Planning**
- Copy existing feature brief → `/feature-spec` → Generate structured specification
- Pattern: Transform rough ideas into clear requirements

## Weekly PM Workflows

**Monday: Strategy Check**
```bash
# Review last week's decisions
/strategy-review weekly-recap.md

# Are we following our guiding policy?
# Do actions still connect to diagnosis?
```

**Wednesday: Stakeholder Sync**
```bash
# Prepare executive update
/stakeholder-sync "executive team update"

# Clear asks, dependencies, timelines
```

**Friday: Research Planning**
```bash
# Plan next week's user interviews
/research-plan "user onboarding feedback"

# Ensure questions connect to real decisions
```

## Document Lifecycle

**1. Draft Creation**
- Start with framework: "Help me create a PRD using the feature-planning prompt"
- Apply structure before writing content

**2. Internal Review** 
- `/prd-review draft-prd.md`
- Fix clarity issues before stakeholder review

**3. Stakeholder Feedback**
- Apply economical-writing to responses
- Use stakeholder-communication for follow-ups

**4. Final Polish**
- One more framework pass before shipping

## Meeting Preparation

**Strategy Reviews**
- Download deck → Apply good-strategy-framework → Prepare pointed questions
- Focus on diagnosis, policy, actions coherence

**Feature Planning**
- Copy rough requirements → `/feature-spec` → Structure before engineering review

**Executive Presentations**
- Apply economical-writing to slide notes
- Cut fluff, lead with conclusions

## Integration Points

This library works with your existing tools:
- **Google Docs**: Copy/paste workflow (see google-docs-integration.md)
- **Notion**: Export pages as markdown, apply frameworks
- **Slack**: Draft messages using stakeholder-communication principles
- **Figma**: Apply user-research discipline to design reviews

The goal: systematic thinking becomes automatic.