# Classic Light (IntelliJ-inspired) — a Zed theme

A light theme for [Zed](https://zed.dev) that ports the color values of
JetBrains IntelliJ's **"Classic Light"** editor color scheme (the legacy
*Default* scheme, presented as *Classic Light* in the New UI).

The palette is taken directly from JetBrains' own
[`DefaultColorSchemesManager.xml`](https://github.com/JetBrains/intellij-community/blob/master/platform/platform-resources/src/DefaultColorSchemesManager.xml),
so syntax colors, the caret-row highlight, selection, gutter, diff/VCS status
colors and the terminal ANSI palette match the original.

> **Not affiliated with or endorsed by JetBrains s.r.o.** "JetBrains" and
> "IntelliJ" are trademarks of JetBrains s.r.o. This is an independent,
> community-made color port for Zed.

## Highlights

The defining trait of Classic Light is preserved: most code stays **black**,
and only a few token classes are colored.

| Token | Color | Style |
| --- | --- | --- |
| Keywords | `#000080` | bold |
| Strings | `#008000` | bold |
| Numbers | `#0000ff` | — |
| Comments / doc | `#808080` | italic |
| Fields / constants | `#660e7a` | bold / bold-italic |
| Annotations | `#808000` | — |
| Classes, functions, params, operators | `#000000` | — |

Editor background `#ffffff`, active line `#fffae3`, line numbers `#999999`.
The project panel (sidebar) is white, with a grey fill for the selected entry
and a blue focus ring for the active entry — mirroring IntelliJ's tool window.

## Install

### From the Zed extensions registry

> Not yet published to the registry. Once it is, open the command palette →
> `zed: extensions`, search for **Classic Light (IntelliJ-inspired)**, and install.

### As a dev extension (now)

1. Clone this repo.
2. In Zed, open the command palette (`cmd-shift-p`) → **`zed: install dev extension`**.
3. Select this repo's folder.
4. Open the theme selector (`cmd-k cmd-t`) and pick **Classic Light (IntelliJ-inspired)**.

### Just the theme file

Copy [`themes/classic-light-intellij.json`](themes/classic-light-intellij.json)
into `~/.config/zed/themes/` and select it in the theme picker.

## Pairs well with

JetBrains' default editor font is **JetBrains Mono**; this theme also looks
great with **Fira Code**. In your Zed `settings.json`:

```json
{
  "buffer_font_family": "Fira Code",
  "buffer_font_features": { "calt": true }
}
```

## License

[MIT](LICENSE) © 2026 Stanislav Lashmanov. Color values are derived from
JetBrains' open-source IntelliJ Community scheme (Apache-2.0).
