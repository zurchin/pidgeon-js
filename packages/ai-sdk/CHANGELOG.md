# Changelog

## 1.2.0

- Pidgeon is now Zurchin: this version is published as `@zurchin/ai-sdk`, and the last `@zurchin/ai-sdk` (1.2.0) only re-exports it and says so once.
- The default host is `https://zurchin.com`. pidgeon.ai keeps answering the API for six months.
- The source repository is `zurchin/pidgeon-js`.

## 1.1.0

- `pidgeonTools()` without `apiKey` reads `ZURCHIN_API_KEY`, else `PIDGEON_API_KEY`.

## 1.0.1

- The description, keywords and README lead with email inboxes for AI agents.
  The tools come in the MCP server's new order, Email first.

## 1.0.0

- Rebuilt for the new Pidgeon: the tools are the hosted MCP server's
  (`registerApiTools` in `@zurchin/mcp`), built from its list, so the two
  never differ. Email, Passport, Bouncer, Auth and the account.
- `pidgeonTools({ apiKey, baseUrl, client, only })` and
  `pidgeonToolApproval(tools)`, which asks a person before the destructive
  tools.
- Removed: everything that spoke the old email API at `/api/v1` (addresses,
  `identityId`, `get_setup`, `check_message`, `verify_sender` and the other
  tools of the old server).
