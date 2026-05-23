# Goodlock AI Trading Desk

![Goodlock AI Trading Desk mark](assets/goodlock-mark.svg)

One prompt that launches a human-approved AI trading operations desk with Paperclip, Claude Code, and the TradingView MCP. It is built for research, backtesting, risk review, paper execution, audit logs, and explicit human approval before live capital is touched.

This fork-ready version is branded for Josh Goodlock. The original upstream GitHub links are intentionally preserved until the repo and TradingView MCP are forked under Josh's account.

## Start Here

| Platform | Prompt |
| --- | --- |
| Windows | [prompts/windows.md](prompts/windows.md) |
| Mac | [prompts/mac.md](prompts/mac.md) |
| Linux | [prompts/linux.md](prompts/linux.md) |

For Windows, open [prompts/windows.md](prompts/windows.md), copy everything below the first horizontal rule, paste it into Claude Code, and hit Enter.

For a more polished install experience, open [onboarding/index.html](onboarding/index.html) in your browser. It gives users a professional onboarding flow, setup checklist, risk-gate explanation, and direct links to the platform prompts.

## What It Builds

Goodlock AI Trading Desk creates a Paperclip organization with six specialist agents:

- **CEO** - your direct report. Triage, delegation, board briefings, and escalation.
- **Research Agent** - scans YouTube, arXiv, TradingView ideas, and Reddit for strategy candidates.
- **Backtest Agent** - validates every idea and stores permanent institutional memory.
- **Risk Management Agent** - blocks strategies that fail the agreed risk floor.
- **Execution Agent** - paper-trades by default and only moves live when the Board explicitly approves.
- **Cost Optimizer** - reviews token usage and trims waste without weakening safety-critical work.

The installer also creates the firm directory, configures risk thresholds, connects the TradingView MCP, stores agent IDs, and opens the Paperclip dashboard.

## Why This Is Commercially Useful

This should be positioned as an AI trading operations kit, not a signal-selling product.

- **Free repo** - public trust, adoption, and community contribution.
- **Paid setup pack** - premium prompts, templates, risk policies, example strategies, and troubleshooting guides.
- **Pro version** - richer reporting, more agent templates, broker-paper integrations, and strategy lifecycle workflows.
- **Done-with-you install** - high-ticket setup for traders, educators, and small quant teams.
- **Enterprise desk** - audit trails, multi-user approvals, compliance logs, and custom governance.

The clean positioning:

> An AI trading operations desk that researches, backtests, risk-checks, and paper-trades strategies before a human approves live capital.

## Requirements

- Claude Code running locally.
- Node.js.
- Git for your operating system.
- TradingView Desktop for the TradingView MCP.
- A Claude Code subscription.
- A paid TradingView plan if your workflow requires the desktop MCP features.

## Onboarding Flow

The prompt walks the user through:

1. OS and tool checks.
2. Five-question desk intake.
3. Anthropic API key setup.
4. Paperclip install and organization creation.
5. Firm directory creation.
6. TradingView MCP install.
7. Agent creation through the Paperclip API.
8. Dashboard launch.
9. Verification and first CEO task.

## Guardrails

- Paper trading is the default.
- Live trading requires explicit Board approval.
- Risk thresholds live in `config/risk-thresholds.json`.
- Only the human Board can change risk thresholds.
- The Risk Management Agent and Execution Agent are kept separate.
- Every strategy must pass backtesting and paper-trading review before live execution.

## Custom Teams

During the intake interview, the onboarding agent asks whether to use Josh Goodlock's six-agent setup or a custom team. Custom roles include role name, reporting line, and mandate, then get embedded into the CEO's delegation brief.

More agents mean more token usage, so the Cost Optimizer is included to surface operational cost and prompt bloat.

## Bring Your Own Strategy

In Question 3, choose Option A. Users can describe a strategy, provide a file path, or upload a strategy document. The onboarding agent embeds that context into the CEO, Research, Backtest, and Risk Management workflows.

## Resources

- Paperclip: https://paperclip.ng
- Upstream repo to preserve until forked: https://github.com/jackson-video-resources/paperclip-zero-human-trading-firm
- TradingView MCP to preserve until forked: https://github.com/LewisWJackson/tradingview-mcp-jackson
- Claude Code: https://claude.ai/download
