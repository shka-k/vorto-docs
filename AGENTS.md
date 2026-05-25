# Documentation project instructions

## About this project

- Documentation site for [Vorto](https://github.com/vorto-editor/vorto), a Rust-based modal terminal editor
- Built on [Mintlify](https://mintlify.com); pages are MDX files with YAML frontmatter
- Configuration and navigation live in `docs.json`
- Run `bunx mint dev` to preview locally
- Run `bunx mint broken-links` to check links

## Terminology

- "Vorto" is the editor; refer to it by name, not "the app" or "the tool"
- "grammar" = a tree-sitter grammar installed via `vorto grammar install`
- "LSP server" = the language server binary the user installs separately; "LSP client" = the built-in client that ships in the binary

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Do not frame Vorto as an "X alternative" or write competitor-comparison content that names other editors (Vim, Neovim, Helix). "Vim-style" / "Vim command grammar" is fine as a genre descriptor of what Vorto implements.
- Be accurate about the built-in vs. install-separately split: the editor's capabilities (LSP client, tree-sitter engine, finder, explorer, Copilot integration) ship in the binary, but per-language grammars and LSP server binaries are installed by the user.
