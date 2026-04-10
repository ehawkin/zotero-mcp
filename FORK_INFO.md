# About This Fork and the `secret` Branch

This repository is a fork of [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp),
maintained by [@ehawkin](https://github.com/ehawkin).

## What this fork contains

This fork develops bug fixes and improvements that are submitted upstream as pull
requests. Changes here are tested locally before submission and may include fixes
that have not yet been merged into the official project.

## The `secret` branch

The `secret` branch is the **install target** for the ehawkin variant of the
Zotero MCP installer. When this fork has unreleased fixes ahead of upstream,
`secret` points to a version containing upstream's code plus those fixes.

The name "secret" reflects that this branch is referenced by an undocumented
installer option — not because anything here is private. All code is public.

### Current status (2026-04-10)

**1 commit ahead of upstream.** Based on upstream v0.3.0 (commit `cf3d23f`) plus:

- `d7f34c0` — Configurable annotation limit with pagination support: adds
  `ZOTERO_MCP_ANNOTATION_LIMIT` env var (default 300), `offset` parameter for
  paging through library-wide annotation queries, and tool description guidance
  for context window management.

## Official install

For the stable release, install from the upstream project directly:

```bash
uv tool install zotero-mcp-server
```

Or visit: https://github.com/54yyyu/zotero-mcp
