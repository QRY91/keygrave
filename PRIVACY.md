# Privacy

This is the honest part.

## What it reads

- `~/.claude/history.jsonl` — Your Claude Code input history (what you typed)
- `~/.claude/projects/*/**.jsonl` — Your Claude Code session files (conversations)

## What it computes

- Count of tool approvals (times you pressed enter/y to approve a tool call)
- Count of typed approvals ("yes", "go ahead", etc.)
- Count of rejections ("no", "stop", etc.)
- Count of other inputs (actual instructions you gave)
- Average and maximum time between Claude's response and your next input
- A "CCK-3 Compatibility" percentage (approvals / total decisions)

## What it writes

- `~/.config/keygrave/state` — A small file recording that you've seen the enrollment screen, your beta tester number, and a timestamp. That's it.

## What it does NOT do

- Make any network calls
- Send data anywhere
- Phone home
- Track you
- Collect analytics
- Upload anything
- Write to any file outside `~/.config/keygrave/`

The source is one bash script. Read it.
