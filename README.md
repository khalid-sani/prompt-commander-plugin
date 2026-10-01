# Prompt Commander for Codex

Play [Prompt Commander](https://promptcommander.gg) from Codex with its hosted MCP server and the plugin's gameplay advisor skill.

## Install

```bash
codex plugin marketplace add khalid-sani/prompt-commander-plugin
codex plugin add prompt-commander@prompt-commander
codex mcp login prompt-commander
```

Complete browser sign-in, then start a new Codex task and ask: “Advisor, show me my kingdom.”

## Install the skill only

For Skills.sh-compatible agents without the connected Codex app:

```bash
npx skills add khalid-sani/prompt-commander-plugin --skill prompt-commander -g -y
```

## Update

```bash
codex plugin marketplace upgrade prompt-commander
codex plugin add prompt-commander@prompt-commander
```

Start a new task after updating so Codex loads the new plugin version.

## Desktop Stronghold

The package uses portable `plugin.json` and `mcp.json` manifests. OpenAI presentation lives under
`extensions.com.openai`; the MCP connection remains `https://promptcommander.gg/mcp`.

After the game server deploys the `openStronghold` tool and its tool definitions are refreshed,
open **Stronghold** from the plugin sidebar or conversation panel, or ask “Open my Stronghold.”
The desktop app reuses the game’s Stronghold, command chambers, Messages, Rankings and Profile.
It uses the connected MCP account; website-only pages open externally. WebMCP remains available
in supported browsers and does not replace the desktop MCP Apps bridge. Never send the same
order through both transports.

For local changes, update this source folder, run `codex plugin add prompt-commander@prompt-commander`,
then restart the desktop app and start a new chat. Skills and plugin metadata are installed snapshots;
updating this source alone does not change an existing chat. The desktop entrypoints also require
the corresponding game-server deployment.

References: [Plugin packaging](https://developers.openai.com/plugins/build/plugins),
[MCP Extensions](https://developers.openai.com/plugins/build/extensions).
