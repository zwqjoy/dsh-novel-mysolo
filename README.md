# dsh-novel-mysolo

A single-agent novel-writing plugin for DeepSeek Harness. It provides the `novel-mysolo` agent preset, displayed as **小说创作**.

## What it does

- The main agent writes and reviews directly; it does not launch subagents.
- It keeps eight quality checks: setting and boundaries, characters, chapter contracts, perspective and style, deliverables and continuity, repetitive prose, plot logic and foreshadowing, and physical/time logic.
- Repair attempts are bounded. Unresolved hard issues remain marked as a draft needing repair; the quality bar is not lowered to force a pass.
- It maintains the project's existing story bible, character, timeline, and foreshadowing records.

## Install

1. Download and extract the source from **Code → Download ZIP**, or clone this repository.
2. In DeepSeek Harness, open **Plugins → Add plugin** and choose the extracted `dsh-novel-mysolo` folder. If the dialog asks for a path, enter that folder's absolute path.
3. Select the **小说创作** (`novel-mysolo`) preset when starting a conversation.

Keep the folder in place after installation because the desktop plugin manager may link to it. Restart DeepSeek Harness after changing plugin files.

This plugin has no runtime package dependencies and does not connect to the original `dsh-novel-solo` package or its update feed. It is distributed as source for installation from a local folder; `private: true` in `package.json` prevents accidental npm publication.

## Customize

Edit `template/persona.md` to change writing and review rules. The plugin is intended for DeepSeek Harness `0.2.1-rc.2` or newer, as declared in `package.json`.

## License and attribution

This customization contains code adapted from Tkingxiao's `dsh-novel-solo`. The original MIT copyright and license are retained in [LICENSE](LICENSE), with provenance described in [NOTICE.md](NOTICE.md). The package identity, runtime dependencies, and update path are independent.

This is a community plugin and is not an official DeepSeek Harness product.
