# claude-kit

Personal collection of everything Claude-related: prompts, skills, slash commands, hooks, and notes.

## Structure

```
claude-kit/
├── skills/           # Claude Code skills (.md files)
├── commands/         # custom slash commands
│   └── ship/         # commit and push to remote
├── hooks/            # shell scripts triggered by Claude Code events
│   ├── pre-tool/     # run before a tool call
│   └── post-tool/    # run after a tool call
├── notes/            # observations, patterns, takeaways
└── templates/        # starter templates for new skills, commands, and prompts
```

### Organization principles

- Executable artifacts (`skills/`, `commands/`, `hooks/`) are kept flat — easy to symlink.
- Text artifacts (`notes/`) grow subdirectories as needed.
