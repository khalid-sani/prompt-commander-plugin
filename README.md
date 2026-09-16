# Prompt Commander for Codex

Play [Prompt Commander](https://promptcommander.gg) from Codex with the connected game app and its gameplay advisor skill.

## Install

```bash
codex plugin marketplace add khalid-sani/prompt-commander-plugin
codex plugin add prompt-commander@prompt-commander
```

Start a new Codex task, then ask: “Advisor, show me my kingdom.” Complete the browser sign-in when prompted.

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
