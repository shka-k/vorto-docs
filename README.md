# Vorto documentation

Source for the [Vorto](https://github.com/vorto-editor/vorto) documentation site, built with [Mintlify](https://mintlify.com).

Vorto is a Rust-based modal terminal editor with a built-in LSP client, tree-sitter highlighting, fuzzy finder, file explorer, and GitHub Copilot support — configured from a single TOML file.

## Structure

- `docs.json` — site config, theme, and navigation
- `index.mdx`, `why-vorto.mdx`, `installation.mdx`, `quickstart.mdx` — top-level pages
- `editing/`, `languages/`, `lsp/`, `configuration/` — documentation grouped by topic
- `troubleshooting.mdx` — common problems and fixes
- `changelog/` — one page per release

## Local preview

Run the Mintlify dev server from the repo root (where `docs.json` lives):

```bash
bunx mint dev
```

The preview is served at `http://localhost:3000`.

Check for broken links before opening a PR:

```bash
bunx mint broken-links
```

## Publishing

Changes merged to the default branch deploy to production automatically via the Mintlify GitHub app.
