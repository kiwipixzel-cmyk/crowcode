# crow.code

A terminal-first coding agent written in Python. It reads and edits files, runs your shell, drives git, and can split one project across several AI models working in parallel — all from the command line.

## What it does

crow.code isn't a chat window bolted onto a code editor. It's a full agent loop that lives in your terminal and can actually act on your project: touch files, run commands, execute tests, and talk to whichever model fits the task.

## Features

### Model access
- **Any provider, one interface** — works with Anthropic, OpenAI, Grok, OpenRouter, or a custom endpoint.
- **Model switching mid-session** — change which model is answering without losing the conversation's context.
- **Parallel multi-AI tasks** — assign different models to different jobs inside the same project (e.g. one writes the code, another writes the docs, another reorganizes the folder structure), all running against the same environment.
- **Image input** — hand it a screenshot or diagram and let it reason about what's in it.

### A real dev environment
- **File tools** — reads, writes, and navigates your project's files as part of the conversation.
- **Shell execution** — runs real commands in your terminal.
- **Git integration** — works with your repo directly: diffs, commits, and history are part of its context.
- **Automatic test execution** — runs your test suite after changes so you know immediately if something broke.
- **Skills system** — teach it repeatable playbooks for tasks you do often.
- **Gmail sending** — can send email directly, useful for reports, notifications, or handoffs.
- **Persistent memory** — keeps context and personalization across sessions.
- **Saved, reloadable sessions** — pick up exactly where you left off.

### Slash commands
| Command | What it does |
|---|---|
| `/plan` | Lays out an approach before touching any code. |
| `/diff` | Shows exactly what changed, in context. |
| `/undo` | Rolls back the last change, cleanly. |
| `/bypassy` | Auto-approves actions when you trust the plan. |
| `/hackit` | Runs a security audit on the current code. |
| `/ultramode` | Gives the agent broader control of the local machine. |
| `/gi` | Multi-persona review — several points of view on the same code. |

### Also included
- **Higgsfield image/video generation**
- **Usage and cost tracking**

## Requirements

- Python
- An API key for at least one supported provider (Anthropic, OpenAI, Grok, or OpenRouter), or a custom endpoint

## Status

Actively developed. Interfaces and commands may change.
