# vikunja — OpenClaw Skill

An [OpenClaw](https://openclaw.ai) skill for interacting with a
[Vikunja](https://vikunja.io) task management instance via its REST API.

## Features

- **Projects** — list, get, create
- **Tasks** — list, get, create, update, mark done, delete, relations
- **Labels** — list, create, add/remove on tasks
- **Assignees** — add/remove users on tasks
- **Reminders** — absolute datetime or relative to due/start/end date

## Requirements

- A running Vikunja instance (self-hosted or cloud)
- An API token created under **Settings → API Tokens** in the Vikunja web UI

## Configuration

Set these environment variables in your OpenClaw agent:

| Variable | Description | Example |
|---|---|---|
| `VIKUNJA_BASE_URL` | Base URL of your Vikunja instance | `https://vikunja.example.com` |
| `VIKUNJA_API_TOKEN` | API token with appropriate scopes | `tk_abc123...` |

## Installation

```bash
npx clawhub@latest install vikunja-api
```

Or manually copy the `vikunja/` folder into your OpenClaw skills directory
and restart the session.

## Example interactions

- *"What tasks are due this week?"*
- *"Create a task 'Deploy new release' in my Homelab project due Friday"*
- *"Mark task 42 as done"*
- *"Add the 'urgent' label to task 17"*
- *"Assign me to task 5"*
- *"Set a reminder for task 8 in 2 hours"*

## Contributing

Issues and PRs welcome. If the Vikunja API changes in a way that breaks
something, please open an issue with your Vikunja version and the affected
endpoint.

## License

MIT
