# Board Transition Action

GitHub Action (composite) to transition GitHub Projects v2 board items to a new status.

## Usage

```yaml
- uses: pateketrueke/board-transition-action@main
  with:
    issue-number: 4
    status: "In Review"
    project-number: 2
    owner: pateketrueke
    token: ${{ secrets.PROJECT_TOKEN }}
```

## Inputs

| Input | Required | Description |
|-------|----------|-------------|
| `issue-number` | yes | Issue number to transition |
| `status` | yes | Target status (Todo, Planning, In Progress, In Review, Done) |
| `project-number` | yes | GitHub Projects v2 project number |
| `owner` | yes | Owner of the project (user or org login) |
| `token` | yes | GitHub token with `project` scope |
