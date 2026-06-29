# Polarish

If you're building AI apps and you're tired of handling inference costs or forcing users to pay for yet another AI subscription, this is for you.

Polarish lets your users bring their own AI subscriptions (Codex, Claude Code, etc.) into your app.

You focus on building workflows.  
Your users use the AI they already pay for.

## How to use

First, ask your users to download the Polarish CLI tool and run the command:

```bash
bun add -g @polarish/cli
```

After installation, users must run this command once:

```bash
polarish
```

This first run is compulsory and will guide them through installing and signing in to Codex and Claude Code.

```bash
polarish origins add https://app.example.com
```

That's it. Now, as a developer, use the Polarish [ai package](./packages/ai/README.md) to build your AI app.

## Important

Polarish wraps around Codex and Claude Code, so it is really important that your users have Codex and Claude Code installed and signed in.

- Codex setup: follow this [link](https://developers.openai.com/codex/cli)
- Claude Code setup: follow this [link](https://claude.com/product/claude-code)

Polarish is heavily inspired by [t3code](https://github.com/pingdotgg/t3code) and [pi-mono](https://github.com/badlogic/pi-mono/) ❤️‍🔥
