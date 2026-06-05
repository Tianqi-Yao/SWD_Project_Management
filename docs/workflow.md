# Task Management Workflow

## How Tasks Are Managed

All tasks are created as GitHub Issues and tracked on the [Kanban Board](https://github.com/users/Tianqi-Yao/projects/2). Claude Code handles all issue and project operations — just describe the update in conversation.

## Kanban Columns

```
Todo → In Progress → Done
```

Tasks move through columns as work progresses. Only move a task to **Done** when the work is fully complete and verified.

## Creating a New Task

Tell Claude:
> "Add a new task to P1: [task description], priority High, start June 10"

Claude will:
1. Create a GitHub Issue with the correct `[Px]` prefix
2. Add it to the Kanban board
3. Set Status, Project, Priority, Start Date, and End Date fields

## Updating Task Status

Tell Claude:
> "Mark #22 as In Progress" or "I finished the segmentation task, close it"

## Issue Naming Convention

```
[P1] Phase 1: Dataset Collection & Annotation
[P2] South Farm Deployment
```

Format: `[Px] <Phase or category>: <Brief description>`

## Project IDs

| ID | Project Name |
|----|-------------|
| P1 | SWD Vision |
| P2 | IoT Paper |
| P3 | Prediction |
| P4 | Robotics |
| P5 | 3DGS |
| P6 | DualCam |

## Useful Commands (for manual use)

```bash
# View all open issues
gh issue list --repo Tianqi-Yao/SWD_Project_Management

# View Kanban board in terminal
gh project view 2 --owner Tianqi-Yao

# Close an issue
gh issue close <NUMBER> --repo Tianqi-Yao/SWD_Project_Management
```
