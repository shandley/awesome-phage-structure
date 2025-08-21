# Contributing to Awesome Phage Structure

Thank you for your interest in contributing to Awesome Phage Structure! This curated list aims to be the go-to resource for AI and machine learning tools in phage structural biology. Your contributions help the phage research community stay current with rapidly evolving computational tools.

## 📋 Table of Contents

- [How to Contribute](#how-to-contribute)
- [Tool Inclusion Criteria](#tool-inclusion-criteria)
- [Submission Format](#submission-format)
- [Pull Request Process](#pull-request-process)
- [Updating Existing Entries](#updating-existing-entries)
- [Reporting Issues](#reporting-issues)
- [Code of Conduct](#code-of-conduct)

## 🤝 How to Contribute

We welcome several types of contributions:

1. **Adding new tools** - Submit AI/ML tools relevant to phage structure and function
2. **Updating existing entries** - Fix broken links, update versions, or improve descriptions
3. **Adding resources** - Suggest tutorials, papers, databases, or communities
4. **Improving organization** - Propose new categories or better categorization
5. **Fixing errors** - Report and fix typos, incorrect information, or dead links

## ✅ Tool Inclusion Criteria

To maintain quality and relevance, tools should meet these criteria:

### Required Criteria

- **Relevance**: Directly applicable to phage/viral structural biology or functional annotation
- **Availability**: Publicly accessible (open source preferred, commercial tools accepted if they offer academic licenses)
- **Functionality**: Working and maintained (last update within 2 years, unless it's a stable, widely-used tool)
- **Documentation**: Clear installation and usage instructions available
- **Scientific Validity**: Peer-reviewed publication or preprint, OR significant community adoption

### Preferred Criteria

- Open source with permissive license
- Provides API or command-line interface
- Includes example data or tutorials
- Active community or support channel
- Benchmarked against other tools

### Not Accepted

- Tools behind complete paywalls with no academic access
- Abandoned projects (>3 years without updates and reported as non-functional)
- Tools without any documentation
- General-purpose tools without clear phage/viral applications

## 📝 Submission Format

When adding a new tool, please follow this format:

```markdown
- **[Tool Name](URL)** `[installation methods]` - Brief, clear description of what the tool does `[Year]`
  - Key feature or unique capability
  - Optional: Link to publication or documentation
```

### Examples

```markdown
- **[PhageTool](https://github.com/example/phagetool)** `[pip, conda]` - Predicts phage receptor binding domains using transformer models `[2024]`
  - Achieves 95% accuracy on benchmark dataset
  - Paper: [Nature Methods](https://doi.org/example)
```

### Format Guidelines

- **Tool Name**: Use official name with correct capitalization
- **URL**: Link to official repository, website, or documentation
- **Installation**: List primary installation methods in backticks: `[pip]`, `[conda]`, `[docker]`, `[web]`, `[source]`
- **Description**: 10-20 words explaining the tool's primary function
- **Year**: Year of latest significant update in backticks: `[2024]`
- **Sub-points**: Optional additional details, keep to 1-2 lines

## 🔄 Pull Request Process

1. **Fork the repository** to your GitHub account

2. **Create a feature branch** with a descriptive name:
   ```bash
   git checkout -b add-phagetool
   git checkout -b fix-broken-links
   git checkout -b update-alphafold-section
   ```

3. **Make your changes** following the format guidelines above

4. **Verify your additions**:
   - [ ] Links work and point to correct resources
   - [ ] Tool meets inclusion criteria
   - [ ] Format matches existing entries
   - [ ] Placed in appropriate category
   - [ ] No duplicate entries

5. **Commit with clear message**:
   ```bash
   git commit -m "Add PhageTool to Structure Prediction section"
   git commit -m "Update AlphaFold3 description and add web server link"
   git commit -m "Fix broken link to BFVD database"
   ```

6. **Submit Pull Request** with:
   - Clear title describing the change
   - Brief description of what you're adding/changing
   - Any relevant context (e.g., "I'm the tool developer" or "This fixes issue #23")

### PR Template

```markdown
## Type of Change
- [ ] New tool addition
- [ ] Update existing entry
- [ ] Fix broken link
- [ ] Add new resource
- [ ] Improve organization

## Description
Brief description of changes

## Checklist
- [ ] Links verified working
- [ ] Follows format guidelines
- [ ] Meets inclusion criteria
- [ ] No duplicates

## Additional Context
(Optional: relationship to tool, how you've used it, etc.)
```

## 🔧 Updating Existing Entries

When updating existing tools:

1. **Version updates**: Update the year tag and any significant changes
2. **URL changes**: Update if repository moved or website changed
3. **Description improvements**: Keep concise while improving clarity
4. **Deprecation**: If a tool is deprecated, mark it clearly:
   ```markdown
   - **[OldTool](URL)** `[DEPRECATED]` - Original description `[2021]`
     - Note: Superseded by [NewTool](#link)
   ```

## 🐛 Reporting Issues

Found a problem but can't fix it yourself? Open an issue with:

1. **Broken Links**: Include the tool name and broken URL
2. **Incorrect Information**: Specify what's wrong and provide correction if known
3. **Tool Suggestions**: Use the issue template to suggest tools you'd like added
4. **Category Suggestions**: Propose new categories or reorganization

### Issue Template

```markdown
## Issue Type
- [ ] Broken link
- [ ] Incorrect information
- [ ] Tool suggestion
- [ ] Category suggestion
- [ ] Other

## Description
Clear description of the issue or suggestion

## Proposed Solution
(If applicable)
```

## 🌟 Quality Guidelines

To maintain the list's quality:

- **Research before adding**: Check if the tool is already listed under a different name
- **Test when possible**: If you can quickly test the tool, verify it works
- **Be objective**: Avoid promotional language; stick to factual descriptions
- **Stay focused**: Keep descriptions concise and relevant
- **Update responsibly**: When updating others' contributions, preserve useful information

## 📜 Code of Conduct

By contributing, you agree to:

- Be respectful and constructive in all interactions
- Welcome newcomers and help them contribute
- Accept constructive criticism gracefully
- Focus on what's best for the phage research community
- Show empathy towards other contributors

## 🙏 Recognition

All contributors will be recognized in our README. Significant contributors may be invited to become repository maintainers.

## 💬 Questions?

If you have questions about contributing:

1. Check existing issues and PRs for similar questions
2. Open a new issue with the "question" label
3. Reach out to the maintainer: [@shandley](https://github.com/shandley)

---

Thank you for helping make Awesome Phage Structure a valuable resource for the phage research community! 🦠🔬