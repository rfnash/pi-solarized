# pi-solarized

A [Solarized](https://ethanschoonover.com/solarized/) Light and Dark color theme
for the [pi coding agent](https://pi.dev), packaged as an installable pi
package.

It provides two themes that share the same canonical Solarized palette
(`base00`–`base3` plus `yellow`, `orange`, `red`, `magenta`, `violet`, `blue`,
`cyan`, `green`) mapped onto pi's UI, markdown, diff, syntax, and thinking-level
tokens:

- **`solarized-light`** — light terminal background (`base3` `#fdf6e3`),
  `base00` foreground.
- **`solarized-dark`** — dark terminal background (`base03` `#002b36`),
  `base0` foreground.

Pick the one matching your terminal's background. Colors assume a matching
background and will have poor contrast on the opposite type.

## Install

```bash
pi install git:github.com/rfnash/pi-solarized
```

## Activate

In `/settings` set the theme to `solarized-light` or `solarized-dark`, or in
`settings.json`:

```json
{
  "theme": "solarized-light"
}
```

Reload with `/reload` (or just restart pi). The theme hot-reloads if you edit
the file while it is active.

## Files

- `themes/solarized-light.json` — the light theme
- `themes/solarized-dark.json` — the dark theme
- `package.json` — pi package manifest (`pi.themes` entry)

## Notes

Solarized Light expects a **light** terminal background (`base3` `#fdf6e3`)
and Solarized Dark expects a **dark** terminal background (`base03` `#002b36`).
All foreground colors assume a matching background and will have poor contrast
on the opposite type.
