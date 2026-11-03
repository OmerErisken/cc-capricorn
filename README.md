# cc-capricorn

A [Claude Code](https://code.claude.com) theme inspired by Capri, the AI character from *Cyberpunk: Edgerunners* season 2. It uses crimson, acid green, electric blue and violet on an ink-black background.

It also includes a matching Windows Terminal color scheme.

## Palette

| Swatch | Hex | Role |
| :- | :- | :- |
| Crimson | `#FC1148` | Main accent: spinner, input box border, usage meter |
| Hot pink | `#FC67A8` | Shimmer, memory, `!` shell border, accept-edits mode |
| Acid green | `#01FE68` | Inline code, dialog borders, success, auto mode, mascot |
| Electric blue | `#3D8BFF` | Plan mode, IDE indicator, system spinner |
| Violet | `#B44DFF` | Skills, merged PRs, text selection |
| Ink | `#090416` | Terminal background, text on colored badges |
| White | `#F8F9F9` | Main text |

Your messages sit on a deep crimson tint (`#2A0712`), and the `ultrathink` rainbow runs crimson → pink → green → blue → violet.

## Install

### Claude Code theme

1. Copy `themes/capricorn.json` into `~/.claude/themes/`. Create the folder if it doesn't exist.
   - macOS / Linux: `~/.claude/themes/capricorn.json`
   - Windows: `%USERPROFILE%\.claude\themes\capricorn.json`
2. Run `/theme` in Claude Code and pick **Capri**.

If the `themes` folder didn't exist before, restart Claude Code once. After that, edits to the file apply to a running session.

### Windows Terminal color scheme (optional)

Claude Code doesn't control your terminal's own background. For the full look, add the matching scheme:

1. Copy `themes/windows-terminal/capricorn.json` to
   `%LOCALAPPDATA%\Microsoft\Windows Terminal\Fragments\Capricorn\capricorn.json`.
2. Close every Windows Terminal window and reopen it.
3. Open **Settings**, choose your profile, then go to **Appearance → Color scheme**, pick **Capri** and click **Save**.

The scheme is loaded as a [fragment](https://learn.microsoft.com/windows/terminal/json-fragment-extensions), so your `settings.json` stays untouched. To remove it, delete the file.

For other terminals, set the background to `#090416` or copy the 16 ANSI colors from the Windows Terminal file.

## Notes

- Claude Code colors the "auto mode on" indicator with the `warning` token. Auto mode is acid green in this theme, so warnings are green too, the same as success messages. Only the ⚠ and ✔ icons tell them apart.
- Errors use `#FF4D4D`, which sits close to the crimson accent.

*Cyberpunk: Edgerunners* and its characters belong to their respective owners. This is an unofficial fan theme and isn't affiliated with them.
