# Board Transition Action

GitHub Action (composite) to transition GitHub Projects v2 board items to a new status.

## Usage

```yaml
- uses: agave/board-transition-action@v1
  with:
    pr-url: https://github.com/agave/example/pull/123
    status: "In Review"
    project-number: 10
    owner: agave
    token: ${{ secrets.PROJECT_TOKEN }}
```

## Inputs

| Input | Required | Description |
|-------|----------|-------------|
| `pr-url` | yes | Pull request URL to add and transition |
| `status` | yes | Target status (Todo, Planning, In Progress, In Review, Done) |
| `project-number` | yes | GitHub Projects v2 project number |
| `owner` | yes | Owner of the project (user or organization login) |
| `token` | yes | GitHub token with `project` scope |
