# Git Commit Convention Rule

When creating or proposing Git commits in any project, strictly adhere to the [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) specification:

### Format Structure
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Requirements
- **Types**:
  - `feat`: A new feature
  - `fix`: A bug fix
  - `docs`: Documentation only changes
  - `style`: Changes that do not affect the meaning of the code (formatting, missing semi-colons, etc.)
  - `refactor`: A code change that neither fixes a bug nor adds a feature
  - `perf`: A code change that improves performance
  - `test`: Adding missing tests or correcting existing tests
  - `build`: Changes that affect the build system or external dependencies
  - `ci`: Changes to CI configuration files and scripts
  - `chore`: Other changes that don't modify src or test files
  - `revert`: Reverting a previous commit
- **Scope**: Optional, enclosed in parentheses, indicating the affected module or area (e.g. `feat(parser): add support for...`).
- **Description**: Concise, imperative, lowercase, no trailing period.
- **Breaking Changes**: Indicated with a `!` preceding the colon (e.g. `feat(api)!: remove deprecated method`) and/or `BREAKING CHANGE: <description>` in the footer.
- **Body & Footer**: If present, separated by blank lines from previous sections.
