# n8n-nodes-nifty

An [n8n](https://n8n.io) community node for [Nifty](https://niftypm.com): create and update tasks, subtasks,
lists, labels, statuses, comments, checklists and custom field values, find projects, members, lists, labels,
statuses and tasks, and start workflows when a task is created, a task is completed or a project is created.

## Installation

In n8n, open **Settings > Community Nodes**, choose **Install** and enter `@nifty-technologies/n8n-nodes-nifty`.
See the n8n [community nodes installation guide](https://docs.n8n.io/integrations/community-nodes/installation/).

## Nodes

- **Nifty**: actions and searches on tasks, subtasks, lists, labels, statuses, comments, checklists, files,
  assignees and custom field values.
- **Nifty Trigger**: a polling trigger for New Task, Task Completed and New Project.

## Credentials

Both nodes have an **Authentication** option that picks one of two credentials:

- **Nifty OAuth2 API** (default, for n8n Cloud): OAuth 2.0 authorization code with PKCE. Enter the client ID and
  client secret of your Nifty OAuth app.
- **Nifty API** (for self-hosted n8n): a personal access token (`nft_user_…`) created under
  **Settings > API Tokens** in Nifty, sent as `Authorization: Bearer <token>`.

The node calls the Nifty v3 API at `https://openapi.niftypm.com/api/v3`.
See [developers.niftypm.com](https://developers.niftypm.com).

## Development

```sh
npm install
npm run build
npm run lint
```

## License

[MIT](LICENSE.md)
