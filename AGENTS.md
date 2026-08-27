## Skill Conventions

- Read and follow the [Claude prompting best practices](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices.md) when writing skills.
- Use `general-purpose` sub-agents for task delegation instead of defining custom, named sub-agents for better compatibility across harnesses. Include an `assets/<task-name>-prompt.md` in the skill for the `general-purpose` sub-agent to use.
- Keep reusable skills caller-agnostic: callers inject workflow-specific context and exceptions; callees define only their reusable contract and behavior.

## Development

When plugin skills change, bump the version in every corresponding `plugin.json` manifest.

## Resources/Documentation

Skills and other plugin components should be designed for compatibility with Claude Code and ChatGPT. See relevant documentation below:

- [Claude Code](https://code.claude.com/docs/en/tools-reference.md)
- [Claude Skills](https://code.claude.com/docs/en/skills.md)
- [ChatGPT Skills](https://learn.chatgpt.com/docs/build-skills.md)
