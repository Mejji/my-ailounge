# Jira Manager Agent Configuration

* agent prompt: [jira-manager](.opencode/agent/jira-manager.md) will be managing these tickets
* only focus on Jira project 'MYD: MY Software Engineering'
* only interact with Jira project 'MYD: MY Software Engineering'
* unresolved tickets only
* put the manipulated tickets with actions in [agents/jira-manager/TODO.md](agents/jira-manager/TODO.md)
* always ask which specific tickets/issue IDs to change (i.e. MYD-1, MYD-2)

## Tickets

### Jira Tickets Snapshot 11-19-2025

[Jira: Current Ticket List (Google Sheet)](https://docs.google.com/spreadsheets/d/1S-w4f6N9F84pUDXVKQdRqiqqvnjcf8vGxhxujmlG8dg/edit?gid=1806480038#gid=1806480038)

### Jira API Reference

* "projectIdOrKey":"MYD"

## Statuses
*from `statuses.json`*

| ID | Name |
|---|---|
| 10000 | To Do |
| 3 | In Progress |
| 10001 | Done |
| 10010 | Blocked |
| 10029 | Staging |

