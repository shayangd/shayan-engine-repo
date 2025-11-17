description: Orchestrated workflow for: Create designer.md documentation file
argument-hint: "<task_path>"
---
# Context
This workflow command was dynamically created to orchestrate agents for:

**Create designer.md documentation file**

1. Create designer.md file at repository root
2. Add Introduction section describing designers and their role
3. Add section about Design Disciplines with subsections
4. Add Skills and Competencies section detailing key abilities
5. Add Tools and Technologies section listing design software
6. Add Design Process section outlining typical workflow
7. Add Career and Industry section with information about professional paths
8. Include reference to 'shayan-engine-repo' in the content
9. Follow markdown formatting conventions used in other documentation files
10. Use proper headers, lists, and tables where appropriate

Parent Task: Generate designer.md file at root level

# Workflow
This command orchestrates the following agent sequence:

1. **documentation-analyst-writer** analyzes requirements and current codebase
2. **documentation-analyst-writer** executes: Create designer.md file at repository root
3. **code-reviewer** executes: Add Introduction section describing designers and their role
4. **code-reviewer** executes: Add section about Design Disciplines with subsections
5. **code-reviewer** executes: Add Skills and Competencies section detailing key abilities
6. **code-reviewer** executes: Add Tools and Technologies section listing design software
7. **code-reviewer** executes: Add Design Process section outlining typical workflow
8. **code-reviewer** executes: Add Career and Industry section with information about professional paths
9. **code-reviewer** executes: Include reference to 'shayan-engine-repo' in the content
10. **code-reviewer** executes: Follow markdown formatting conventions used in other documentation files
11. **code-reviewer** executes: Use proper headers, lists, and tables where appropriate

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
