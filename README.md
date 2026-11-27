# librarium-kit

A Warhammer 40,000 themed fork of [savvy-progress](https://github.com/johnnyvizz/claude-kit/tree/main/plugins/savvy-progress)
for Claude Code, with its companion [savvy-flow](https://github.com/johnnyvizz/claude-kit/tree/main/plugins/savvy-flow),
both by johnnyvizz (MIT; see LICENSE).

**savvy-progress (40K)**: a progress bar above the prompt and a live panel of subagents (`/agents-info`). The crabs
serve the Imperium: a levitating Librarian, an Inquisitor with his rosette, a Tech-Priest with a servo-arm, a Space
Marine with a bolter, a Guardsman with the Imperial banner, a Rogue Trader with a power sword, and a purity-sealed
servitor for everything else. Colours are stone, brass and parchment. **savvy-flow** is upstream, unchanged.

**blast-radius**: Anthropic's [Blast Radius](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/blast-radius)
mod, unchanged (Apache-2.0, see plugins/blast-radius/LICENSE and NOTICE): it holds risky shell commands and shows what
they would delete or discard, with Proceed and Cancel. Needs `bash`, `git`, `find` and `du` on PATH (on Windows: Git
for Windows with its Unix tools on PATH).

**replay-theater**: Anthropic's example mod, unchanged (Apache-2.0): step through the file edits of the last turn one
diff at a time (`/replay`).

## Install (Claude Code)

```
/plugin marketplace add Anzalar1/librarium-kit
/plugin install savvy-progress@librarium-kit
/plugin install savvy-flow@librarium-kit
/plugin install blast-radius@librarium-kit
/plugin install replay-theater@librarium-kit
```

Then restart Claude Code (or run `/reload-plugins`). `/agents-info` shows or hides the panel.
