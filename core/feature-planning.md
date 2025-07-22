# Feature Planning Discipline

*Build what matters. Cut what doesn't.*

## The Prompt

For every feature, write these five sentences:

1. **The problem**: Users cannot _____ because _____
2. **The solution**: We will build _____ so that _____
3. **The feasibility**: Engineering confirms this is _____ (simple/moderate/complex) because _____
4. **The measure**: Success means _____ (one metric)
5. **The cost**: We will not build _____ to make time for this

Apply McCloskey's knife:

- **Kill modifiers** - "Robust," "scalable," "enhanced" say nothing
- **Use active voice** - "This feature will..." not "Users will be enabled to..."
- **Lead with value** - Start with user benefit, not technical approach
- **One feature per spec** - Multiple features mean unclear thinking

## Technical Feasibility Assessment

Before finalizing any feature spec, validate technical approach:

**Engineering review questions:**
- What existing systems/APIs does this touch?
- What new infrastructure is required?
- What are the performance implications?
- What could break or need refactoring?
- How will this scale with user growth?

**Feasibility classification:**
- **Simple**: Uses existing patterns, minimal new code, low risk
- **Moderate**: Some new development, standard complexity, manageable risk
- **Complex**: New architecture, significant unknowns, high technical risk

**Risk mitigation:**
- Prototype critical unknowns first
- Break complex features into smaller phases
- Plan technical spikes for architecture decisions
- Include buffer time for unexpected complexity

## The Test

Can you explain this feature to your grandmother? Can an engineer estimate it confidently? If not to both, rewrite until you can.

## Practice

Delete every adjective from your feature description. Add one sentence about technical complexity. What remains?