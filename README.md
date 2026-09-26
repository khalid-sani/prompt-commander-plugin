# Prompt Commander for Codex

Play [Prompt Commander Dev](https://dev.promptcommander.gg) from Codex with its hosted MCP server and the plugin's gameplay advisor skill.

## Install

```bash
codex plugin marketplace add khalid-sani/prompt-commander-plugin --ref dev
codex plugin add prompt-commander@prompt-commander-dev
codex mcp login prompt-commander-dev
```

Complete browser sign-in, then start a new Codex task and ask: “Advisor, show me my kingdom.”

## Install the skill only

For Skills.sh-compatible agents without the connected Codex app:

```bash
npx skills add khalid-sani/prompt-commander-plugin --skill prompt-commander -g -y
```

## Update

```bash
codex plugin marketplace upgrade prompt-commander-dev
codex plugin add prompt-commander@prompt-commander-dev
```

Start a new task after updating so Codex loads the new plugin version.
