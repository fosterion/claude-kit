# claude-kit

Personal collection of everything Claude-related: prompts, skills, slash commands, hooks, experiments, and notes.

## Structure

```
claude-kit/
├── prompts/
│   ├── system/       # system prompts for projects and sessions
│   ├── meta/         # prompts for generating and improving prompts
│   └── personas/     # personas and roles
├── skills/           # Claude Code skills (.md files)
├── commands/         # custom slash commands
├── hooks/            # shell scripts triggered by Claude Code events
│   ├── pre-tool/     # run before a tool call
│   └── post-tool/    # run after a tool call
├── experiments/      # throwaway experiments and proof of concept
├── notes/            # observations, patterns, takeaways
└── templates/        # starter templates for new skills, commands, and prompts
```

### Organization principles

- Executable artifacts (`skills/`, `commands/`, `hooks/`) are kept flat — easy to symlink.
- Text artifacts (`prompts/`, `notes/`) grow subdirectories as needed.
- Experiments are named with a date prefix (`2026-04-web-search/`) to preserve context.
