# Workflow E2E Test

This repository is used for end-to-end testing of organization-wide workflows.

## Purpose

This repository demonstrates the use of organization-wide workflows for:

1. **Issue Labeling**: Automatically adding labels to issues
2. **PR Status Tracking**: Updating issue labels based on PR status
3. **Contributing Guidelines**: Reminding about contribution guidelines
4. **Label Creation**: Creating standard labels in the repository
5. **CI Failure Reminders**: Reminding about pre-commit hooks on CI failure
6. **Release PR Generation**: Generating release PRs with all pending issues

## Workflows

The following workflows are implemented in this repository:

- `issue-labeler.yml`: Automatically adds a "triage" label to new issues
- `contributing-reminder.yml`: Checks if issues/PRs reference CONTRIBUTING.md
- `pr-status-tracker.yml`: Updates issue labels based on PR status
- `label-creator.yml`: Creates standard labels in the repository
- `ci-failure-reminder.yml`: Reminds about pre-commit hooks on CI failure
- `release-pr-generator.yml`: Generates release PRs with all pending issues

## Testing

This repository is used to test the complete issue lifecycle:

1. **Issue Creation**: Issues are automatically labeled with "triage"
2. **Triage Process**: Issues are manually labeled as "ready-for-development"
3. **Development**: Draft PRs automatically label issues as "in-progress"
4. **Review**: Ready PRs automatically label issues as "review-ready"
5. **Merge to Develop**: Merged PRs automatically label issues as "merged-to-develop"
6. **Release**: Releases automatically label issues as "released"
# Test PR Status Tracker
