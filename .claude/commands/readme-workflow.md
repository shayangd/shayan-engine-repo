description: Orchestrated workflow for: Update README.md with comprehensive project documentation
argument-hint: "<task_path>"
---
# Context
This workflow command was dynamically created to orchestrate agents for:

**Update README.md with comprehensive project documentation**

1. Add detailed project overview section explaining the repository's purpose as a test repository for the Shayan Engine GitHub app
2. Create repository structure section documenting all markdown files (Ball.md, alphabet.md, banana.md, mango.md) and their contents
3. Add setup instructions section with prerequisites and repository cloning steps
4. Create usage examples section demonstrating how to navigate and use the documentation files
5. Add contribution guidelines section explaining the git workflow, branch naming conventions (disrupt-engine/<descriptive-name-with-hash>), and pull request process
6. Include sections for development workflow, testing context, and any additional relevant information
7. Format the README.md professionally with proper markdown syntax, headers, lists, and code blocks

Parent Task: Update README with project information

# Workflow
This command orchestrates the following agent sequence:

1. **documentation-analyst-writer** analyzes requirements and current codebase
2. **documentation-analyst-writer** executes: Add detailed project overview section explaining the repository's purpose as a test repository for the Shayan Engine GitHub app
3. **code-reviewer** executes: Create repository structure section documenting all markdown files (Ball.md, alphabet.md, banana.md, mango.md) and their contents
4. **code-reviewer** executes: Add setup instructions section with prerequisites and repository cloning steps
5. **code-reviewer** executes: Create usage examples section demonstrating how to navigate and use the documentation files
6. **code-reviewer** executes: Add contribution guidelines section explaining the git workflow, branch naming conventions (disrupt-engine/<descriptive-name-with-hash>), and pull request process
7. **code-reviewer** executes: Include sections for development workflow, testing context, and any additional relevant information
8. **code-reviewer** executes: Format the README.md professionally with proper markdown syntax, headers, lists, and code blocks

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
