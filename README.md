# claude-code-plugins

Personal Claude Code plugin marketplace by jchen0824.

## Add This Marketplace

```bash
/plugin marketplace add jchen0824/claude-code-plugins
```

## Available Plugins

### github-devex

GitHub developer experience tools: automated Codex code review loops and PR workflow automation.

**Install:**
```bash
/plugin install github-devex@jchen0824/claude-code-plugins
```

**Skills included:**
- `request-codex-review` — Automate Codex PR review with full fix-and-iterate loops

**Repository:** https://github.com/jchen0824/claude-github-devex

---

## Releasing Plugin Updates

When releasing a new version of a plugin:

1. Tag the plugin repo: `git tag vX.Y.Z && git push --tags`
2. Bump `version` in `.claude-plugin/marketplace.json` to match the tag
3. Commit and push this repo

Users update via:
```bash
/plugin update github-devex@jchen0824/claude-code-plugins
```

> **Note:** The `version` field signals to Claude Code that an update is available. The plugin system fetches the latest commit from the plugin repo's default branch on update.
