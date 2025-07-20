# PM Prompts Test Suite

Comprehensive testing framework for all PM prompts, commands, and frameworks to ensure quality and consistency.

## Test Structure

Tests are organized into categories with specific validation criteria:
- **Input examples** from realistic PM scenarios
- **Expected output validation** with measurable criteria
- **Framework application** verification
- **Edge case handling** and error scenarios
- **Success criteria** for each test case

## Test Categories

### Framework Tests (`frameworks/`)
Core PM frameworks for structured thinking:
- data-analysis.test.md - Data interpretation and insights
- good-strategy-framework.test.md - Rumelt's strategy kernel
- user-research.test.md - Research planning and execution
- feature-planning.test.md - Feature specification discipline
- stakeholder-communication.test.md - Clear stakeholder alignment
- economical-writing.test.md - McCloskey's writing principles
- difficult-conversations.test.md - Structured conflict resolution
- executive-presentations.test.md - C-suite communication
- prfaq-generation.test.md - Amazon-style announcements
- quarterly-planning.test.md - Strategic planning cycles
- strategic-planning.test.md - Long-term strategic documents

### Command Tests (`commands/`)
Slash commands for immediate PM workflow support:
- email.test.md - Stakeholder email generation
- spec.test.md - Feature specification creation
- review.test.md - Document improvement
- meeting-prep.test.md - Meeting planning and facilitation
- focus-discipline.test.md - Priority and focus management
- strategy-check.test.md - Strategy quality assessment
- feature-spec.test.md - Detailed feature specifications
- stakeholder-sync.test.md - Stakeholder communication
- research-plan.test.md - User research planning
- prd-review.test.md - PRD quality improvement
- metrics-clarity.test.md - Data analysis and insights
- pm-help.test.md - Framework guidance and support
- pm-examples.test.md - Example scenarios and applications

### Workflow Tests (`workflows/`)
PM process automation and optimization:
- pm-workflows.test.md - Standard PM process flows
- workflow-automation.test.md - Process automation
- focus-discipline.test.md - Focus and prioritization systems

### Integration Tests (`integration/`)
Tool integrations and cross-platform functionality:
- google-docs-integration.test.md - Google Workspace integration

### Documentation Tests (`documentation/`)
User onboarding and education materials:
- usage-examples.test.md - Framework application examples
- quick-start-guide.test.md - New user onboarding
- installation.test.md - Setup and configuration

## Running Tests

### Quick Start
```bash
# Run complete test suite
./run-all-tests.sh

# Test specific category
ls frameworks/*.test.md
ls commands/*.test.md
```

### Individual Tests
1. Open specific test file
2. Apply test inputs to corresponding PM prompt/command
3. Validate output against expected criteria checklist
4. Document results and any issues

### Test Validation
Each test includes validation checklists:
- [ ] Framework principles correctly applied
- [ ] Professional communication standards met
- [ ] Actionable recommendations provided
- [ ] Edge cases handled appropriately
- [ ] Success criteria met

## Test Quality Standards

- **Realistic scenarios** from actual PM work
- **Measurable validation criteria** for objective assessment
- **Edge case coverage** for robust testing
- **Professional standards** for output quality
- **Actionable results** that improve PM effectiveness

## Maintenance

- **Weekly**: Command functionality verification
- **Monthly**: Framework application review
- **Quarterly**: Complete test suite update
- **Continuous**: Add scenarios based on user feedback

## Getting Started

1. Run `./run-all-tests.sh` for complete validation
2. Start with `quick-start-guide.test.md` for new users
3. Test frameworks relevant to your current PM challenges
4. Use command tests for daily workflow validation

## Success Metrics

- Test pass rate >95%
- User adoption of tested frameworks
- Reduced PM decision-making time
- Improved stakeholder satisfaction

For detailed execution instructions, see `test-runner.md`.