# Shayan Engine Repository

## Project Overview

This repository serves as a comprehensive test environment for the **Shayan Engine** GitHub app. It is designed specifically to validate and demonstrate GitHub app functionality, workflow automation, and integration capabilities. Rather than containing production code, this repository houses curated markdown documentation files that facilitate thorough testing of GitHub operations, pull request workflows, branch management, and automated processes.

The repository provides a safe, controlled environment for:
- Testing GitHub app integrations and webhooks
- Validating automated workflow processes
- Demonstrating pull request creation and management
- Verifying branch naming conventions and git operations
- Testing documentation generation and updates
- Simulating real-world development scenarios in a low-risk setting

## Repository Structure

The repository contains the following markdown documentation files:

### Documentation Files

| File | Description | Content Summary |
|------|-------------|-----------------|
| **Ball.md** | Comprehensive sports ball documentation | Detailed information about 8 different sports balls (cricket, football, basketball, tennis, volleyball, baseball, golf, rugby) including physical properties, specifications, materials, manufacturing processes, care guidelines, and historical background |
| **alphabet.md** | English alphabet reference | Simple listing of all 26 letters of the English alphabet in both uppercase and lowercase format |
| **banana.md** | Banana fruit documentation | Complete guide covering banana varieties (Cavendish, Plantain, Lady Finger, Red Banana, Blue Java), nutritional benefits, major growing regions, and interesting facts |
| **mango.md** | Mango fruit documentation | Detailed information about mango varieties (Alphonso, Tommy Atkins, Kent, Ataulfo, Haden, Keitt), nutritional benefits, cultivation regions, and cultural significance |
| **CLAUDE.md** | Claude Code instructions | Project-specific guidance for Claude Code when working with this repository |
| **README.md** | This file | Main repository documentation and user guide |

## Setup Instructions

### Prerequisites

To work with this repository, you need:

- **Git**: Version control system (version 2.0 or higher recommended)
  ```bash
  git --version
  ```
- **GitHub Account**: Access to create branches and pull requests
- **Text Editor**: Any markdown-compatible editor (VS Code, Sublime Text, Vim, etc.)
- **Basic Git Knowledge**: Understanding of git commands and GitHub workflow

### Cloning the Repository

1. **Clone via HTTPS:**
   ```bash
   git clone https://github.com/shayangd/shayan-engine-repo.git
   cd shayan-engine-repo
   ```

2. **Clone via SSH:**
   ```bash
   git clone git@github.com:shayangd/shayan-engine-repo.git
   cd shayan-engine-repo
   ```

3. **Verify the clone:**
   ```bash
   git status
   git branch
   ```

## Usage Examples

### Navigating Documentation Files

#### Reading Sports Ball Documentation
```bash
# View comprehensive ball documentation
cat Ball.md | less

# Search for specific ball type
grep -A 10 "Tennis Ball" Ball.md

# View physical properties table
sed -n '/Physical Properties/,/Material Composition/p' Ball.md
```

#### Accessing Fruit Documentation
```bash
# Compare banana and mango varieties
grep "##.*Varieties" banana.md mango.md

# View nutritional information
grep -A 15 "Nutritional Benefits" mango.md
```

#### Quick Reference Files
```bash
# Display the alphabet
cat alphabet.md

# List all markdown files
ls -la *.md
```

### Working with the Repository

#### Searching Across All Documentation
```bash
# Find all mentions of "nutrition"
grep -r "nutrition" *.md

# Count total lines of documentation
wc -l *.md

# Search for specific topics
grep -r "vitamin" banana.md mango.md
```

#### Viewing File Metadata
```bash
# Check file sizes
ls -lh *.md

# View last modified dates
ls -lt *.md

# Display file structure
tree -L 1
```

## Contribution Guidelines

### Git Workflow

This repository follows a structured GitHub-based workflow designed to test pull request processes and branch management:

#### Branch Management

1. **Main Branch**:
   - Branch name: `main`
   - Protected branch containing stable documentation
   - All changes must be merged via pull requests

2. **Feature Branches**:
   - **Naming Convention**: `disrupt-engine/<descriptive-name-with-hash>`
   - **Format**: Prefix with `disrupt-engine/`, followed by a descriptive name with words separated by hyphens, ending with a short hash
   - **Examples**:
     - `disrupt-engine/create-ballmd-with-detailed-af896437`
     - `disrupt-engine/update-readme-with-project-1ea52f59`
     - `disrupt-engine/create-alphabetmd-file-with-ae08f1ee`

#### Step-by-Step Contribution Process

1. **Create a Feature Branch**
   ```bash
   # Ensure you're on main and up to date
   git checkout main
   git pull origin main

   # Create a new feature branch following the naming convention
   git checkout -b disrupt-engine/your-descriptive-name-12345678
   ```

2. **Make Your Changes**
   ```bash
   # Edit the relevant markdown file(s)
   vim Ball.md  # or your preferred editor

   # Check your changes
   git diff
   ```

3. **Commit Your Changes**
   ```bash
   # Stage your changes
   git add Ball.md

   # Commit with a descriptive message
   git commit -m "Add volleyball specifications to Ball.md"
   ```

4. **Push to Remote**
   ```bash
   # Push your feature branch to GitHub
   git push -u origin disrupt-engine/your-descriptive-name-12345678
   ```

5. **Create a Pull Request**
   - Navigate to the repository on GitHub
   - Click "Compare & pull request" for your branch
   - Provide a clear title and description
   - Submit the pull request for review

6. **After Merge**
   ```bash
   # Switch back to main and update
   git checkout main
   git pull origin main

   # Optionally delete the local feature branch
   git branch -d disrupt-engine/your-descriptive-name-12345678
   ```

### Commit Message Guidelines

Write clear, descriptive commit messages:

**Good Examples:**
- `Create Ball.md with comprehensive ball documentation`
- `Update README.md with detailed project overview`
- `Add nutritional information to banana.md`

**Avoid:**
- `Update file`
- `Fix stuff`
- `WIP`

### Pull Request Best Practices

- **Clear Titles**: Describe what the PR accomplishes
- **Detailed Descriptions**: Explain the changes and their purpose
- **Single Purpose**: Each PR should address one logical change
- **Review Ready**: Ensure all changes are intentional and complete
- **Test Context**: Since this is a test repository, note what GitHub app functionality the PR is testing

## Development Workflow

### Typical Development Cycle

1. **Identify Task**: Determine what documentation needs to be added or updated
2. **Create Branch**: Follow the `disrupt-engine/<descriptive-name-hash>` naming convention
3. **Implement Changes**: Edit markdown files with new content or corrections
4. **Local Review**: Check markdown formatting and content accuracy
5. **Commit**: Create descriptive commits for your changes
6. **Push**: Upload your branch to GitHub
7. **Pull Request**: Create PR to merge into `main`
8. **Review**: Wait for review and address any feedback
9. **Merge**: Once approved, merge via GitHub interface
10. **Cleanup**: Delete feature branch and update local `main`

### Markdown Formatting Standards

When editing or creating markdown files, follow these standards:

- Use `#` for main title (H1)
- Use `##` for major sections (H2)
- Use `###` for subsections (H3)
- Include blank lines between sections
- Use tables for structured data
- Use code blocks with language specification
- Use bullet points for lists
- Include line breaks for readability

## Testing Context

### Purpose as Test Repository

This repository is specifically designed to facilitate testing of the **Shayan Engine** GitHub app. Key testing scenarios include:

#### GitHub App Integration Testing
- **Webhook Events**: Testing app responses to push, pull request, and branch events
- **API Interactions**: Validating GitHub API calls and responses
- **Automation Workflows**: Testing automated processes triggered by repository events

#### Pull Request Workflow Testing
- **PR Creation**: Testing automated PR generation
- **Branch Management**: Validating branch naming and lifecycle management
- **Merge Strategies**: Testing different merge approaches and conflict resolution

#### Documentation Operations
- **File Creation**: Testing creation of new markdown documentation
- **File Updates**: Validating updates to existing documentation
- **Content Generation**: Testing automated content generation capabilities

### Testing Guidelines

When using this repository for testing:

1. **Isolated Changes**: Keep test changes isolated to avoid conflicts
2. **Clear Documentation**: Document what each test PR is validating
3. **Revertability**: Ensure test changes can be easily reverted if needed
4. **Non-Breaking**: Test changes should not break existing documentation structure
5. **Descriptive Commits**: Use commit messages that explain the test purpose

## Additional Information

### Repository Maintenance

- **Regular Updates**: Documentation files may be updated to test various scenarios
- **Branch Cleanup**: Feature branches are deleted after merge to keep repository clean
- **Main Protection**: The `main` branch is protected and requires PR for changes

### Support and Questions

For questions about:
- **Repository Usage**: Refer to this README and CLAUDE.md
- **GitHub App Issues**: Contact the Shayan Engine maintainers
- **Contribution Process**: Review the Contribution Guidelines section above

### License

This repository is maintained for testing purposes. Please consult with repository administrators regarding usage rights.

---

**Last Updated**: 2025-11-21
**Repository Purpose**: Testing environment for Shayan Engine GitHub app
**Main Branch**: `main`
**Branch Naming Convention**: `disrupt-engine/<descriptive-name-with-hash>`
