# PM Prompts Test Runner

## Overview
This document provides a comprehensive testing framework for all PM prompts and commands. Tests are organized by category and can be run individually or as a complete suite.

## Test Categories

### Framework Tests
Test core PM frameworks for consistency and effectiveness:
- `frameworks/data-analysis.test.md` - Data interpretation and insight generation
- `frameworks/good-strategy-framework.test.md` - Rumelt's strategy kernel application
- `frameworks/user-research.test.md` - Research planning and execution
- `frameworks/feature-planning.test.md` - Feature specification discipline
- `frameworks/stakeholder-communication.test.md` - Clear stakeholder alignment
- `frameworks/economical-writing.test.md` - McCloskey's writing principles
- `frameworks/difficult-conversations.test.md` - Structured conflict resolution
- `frameworks/executive-presentations.test.md` - C-suite communication
- `frameworks/prfaq-generation.test.md` - Amazon-style announcements
- `frameworks/quarterly-planning.test.md` - Strategic planning cycles
- `frameworks/strategic-planning.test.md` - Long-term strategic documents

### Command Tests
Test slash commands for immediate PM workflow support:
- `commands/email.test.md` - Stakeholder email generation
- `commands/spec.test.md` - Feature specification creation
- `commands/review.test.md` - Document improvement
- `commands/meeting-prep.test.md` - Meeting planning and facilitation
- `commands/focus-discipline.test.md` - Priority and focus management
- `commands/strategy-check.test.md` - Strategy quality assessment
- `commands/feature-spec.test.md` - Detailed feature specifications
- `commands/stakeholder-sync.test.md` - Stakeholder communication
- `commands/research-plan.test.md` - User research planning
- `commands/prd-review.test.md` - PRD quality improvement
- `commands/metrics-clarity.test.md` - Data analysis and insights
- `commands/pm-help.test.md` - Framework guidance and support
- `commands/pm-examples.test.md` - Example scenarios and applications

### Workflow Tests
Test PM workflow automation and processes:
- `workflows/pm-workflows.test.md` - Standard PM process flows
- `workflows/workflow-automation.test.md` - Process automation and optimization
- `workflows/focus-discipline.test.md` - Focus and prioritization systems

### Integration Tests
Test tool integrations and cross-platform functionality:
- `integration/google-docs-integration.test.md` - Google Workspace integration

### Documentation Tests
Test user onboarding and education materials:
- `documentation/usage-examples.test.md` - Framework application examples
- `documentation/quick-start-guide.test.md` - New user onboarding
- `documentation/installation.test.md` - Setup and configuration

## Running Tests

### Individual Test Execution
1. Open specific test file (e.g., `frameworks/good-strategy-framework.test.md`)
2. Use test inputs with corresponding PM prompt/command
3. Validate output against expected criteria
4. Mark validation checklist items as pass/fail
5. Document any issues or improvements needed

### Framework Test Suite
Run all framework tests to ensure core PM discipline consistency:
```bash
# Test all core frameworks
for test in frameworks/*.test.md; do
    echo "Testing $(basename $test)"
    # Apply test inputs and validate outputs
done
```

### Command Test Suite
Test all slash commands for immediate workflow support:
```bash
# Test all commands
for test in commands/*.test.md; do
    echo "Testing $(basename $test)"
    # Execute commands and validate responses
done
```

### Complete Test Suite
Run all tests for comprehensive validation:
```bash
# Full test suite execution
./run-all-tests.sh
```

## Test Quality Standards

### Input Quality
- Realistic PM scenarios
- Appropriate complexity level
- Clear context and constraints
- Relevant stakeholder information

### Output Validation
- Measurable success criteria
- Framework application accuracy
- Professional communication standards
- Actionable recommendations

### Edge Case Coverage
- Resource constraints
- Time pressure situations
- Stakeholder conflicts
- Technical limitations

## Test Maintenance

### Regular Review Schedule
- **Weekly**: Command functionality tests
- **Monthly**: Framework application tests
- **Quarterly**: Complete test suite review

### Updating Tests
1. Review user feedback and common issues
2. Add new test scenarios based on real usage
3. Update validation criteria as frameworks evolve
4. Ensure test coverage for new features

### Success Metrics
- Test pass rate >95%
- User adoption of tested frameworks
- Reduced PM decision-making time
- Improved stakeholder satisfaction

## Getting Started
1. Choose relevant test category for your needs
2. Start with quick-start-guide tests for new users
3. Progress to framework tests for core PM skills
4. Use command tests for daily workflow validation
5. Run integration tests for tool setup validation

## Support
- Issues: Document in test results
- Improvements: Submit via framework feedback
- New scenarios: Add to relevant test files
- Questions: Reference pm-help command tests