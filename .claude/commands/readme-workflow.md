description: Orchestrated workflow for: Expand README.md with comprehensive documentation sections
argument-hint: "<task_path>"
---
# Context
This workflow command was dynamically created to orchestrate agents for:

**Expand README.md with comprehensive documentation sections**

1. Add clear project description explaining the shayan-engine GitHub app testing repository
2. Add installation instructions section (covering prerequisites and setup steps)
3. Add usage examples section (demonstrating how to use the repository for GitHub app testing)
4. Add configuration details section (explaining any setup or environment configuration)
5. Add contributing guidelines section (including how to contribute, code standards, and PR process)
6. Add license information section (specifying the repository license)
7. Ensure proper markdown formatting with clear headings, lists, and code blocks where appropriate

Parent Task: Update README documentation

# Workflow
This command orchestrates the following agent sequence:

1. **documentation-analyst-writer** analyzes requirements and current codebase
2. **documentation-analyst-writer** executes: Add clear project description explaining the shayan-engine GitHub app testing repository
3. **code-reviewer** executes: Add installation instructions section (covering prerequisites and setup steps)
4. **code-reviewer** executes: Add usage examples section (demonstrating how to use the repository for GitHub app testing)
5. **code-reviewer** executes: Add configuration details section (explaining any setup or environment configuration)
6. **code-reviewer** executes: Add contributing guidelines section (including how to contribute, code standards, and PR process)
7. **code-reviewer** executes: Add license information section (specifying the repository license)
8. **code-reviewer** executes: Ensure proper markdown formatting with clear headings, lists, and code blocks where appropriate

# Agents Orchestrated
- **documentation-analyst-writer**: Technical documentation creation
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
