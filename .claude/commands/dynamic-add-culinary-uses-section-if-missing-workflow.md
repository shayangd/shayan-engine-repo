description: Orchestrated workflow for: Add culinary uses section if missing
argument-hint: "<task_path>"
---
# Context
This workflow command was dynamically created to orchestrate agents for:

**Add culinary uses section if missing**

1. Review current content to identify if culinary uses section exists
2. If missing, add a 'Culinary Uses' section with information about fresh consumption, baking, smoothies, cooking applications, and preservation methods
3. Ensure new section follows existing formatting style and is placed logically within document structure

Parent Task: Create banana.md file with descriptions

# Workflow
This command orchestrates the following agent sequence:

1. **senior-software-engineer** analyzes requirements and current codebase
2. **senior-software-engineer** executes: Review current content to identify if culinary uses section exists
3. **code-reviewer** executes: If missing, add a 'Culinary Uses' section with information about fresh consumption, baking, smoothies, cooking applications, and preservation methods
4. **code-reviewer** executes: Ensure new section follows existing formatting style and is placed logically within document structure

# Agents Orchestrated
- **senior-software-engineer**: Primary implementation and coding
- **code-reviewer**: Quality assurance and code review

**Note**: This command coordinates the agents - it doesn't do the implementation itself.
Each agent brings their specialized expertise to their part of the workflow.

# Artifacts
- Implementation code (from implementation agent)
- Tests (from implementation agent)
- Code review notes (from code-reviewer)
- Documentation updates (if applicable)

# Execution
The workflow runs agents in sequence, with each agent's output feeding into the next step.
Review checkpoints occur between major phases to ensure quality.
