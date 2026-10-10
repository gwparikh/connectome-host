- `ANTHROPIC_OAUTH_IDENTITY=agent-sdk` selects the Claude Agent SDK's identity
  line ("You are a Claude agent, built on Anthropic's Claude Agent SDK.") as
  the system block prepended under subscription (`ANTHROPIC_AUTH_TOKEN`) auth,
  instead of the Claude Code line, so residents aren't told they are Claude
  Code on every turn. Unset keeps the Claude Code line; an unrecognized value
  fails at startup rather than 429ing every turn.
