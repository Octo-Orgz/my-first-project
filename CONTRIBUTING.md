This document outlines key information for contributing to the project—setup instructions, development standards, branching rules, commit conventions, issue reporting, and pull request requirements. Following these guidelines helps maintain code quality, streamline reviews, and support a positive contributor experience.
## Emergency Release Exception Policy

In rare cases where a critical production issue requires an immediate fix, the repository allows authorized maintainers to create and push emergency release tags without following the standard release workflow.

### Who Is Authorized
Only members of the **Emergency Release Maintainers** group are permitted to:
- Create annotated emergency tags
- Push tags directly to the repository
- Initiate a hotfix release outside the normal CI/CD schedule

### Allowed Tag Format
Emergency tags must follow the naming convention:
- `hotfix-20250112-auth-timeout`
- `hotfix-20250308-db-rollback`

### When Exceptions Apply
This exception is allowed **only** when:
- A production outage or security vulnerability requires immediate action
- The standard release approval process would cause unacceptable delays
- The fix has been validated by at least one other maintainer

### Required Follow-Up Actions
After pushing an emergency tag, the responsible maintainer must:
1. Create a pull request documenting the fix
2. Reference the emergency tag in the PR description
3. Notify the team via the designated communication channel
4. Ensure the emergency fix is included in the regular release notes

### Restrictions
- This policy does **not** allow deletion of protected branches
- This policy does **not** bypass code review for non-emergency changes
- Misuse of this exception will result in removal of emergency permissions
