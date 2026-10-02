# Solarized for Actual Budget

A dark theme for [Actual Budget](https://actualbudget.org), a port of the
[Solarized](https://github.com/solarized) colour scheme. Forked from palenight, in progress.

| | |
| --- | --- |
| ![#292d3e](https://placehold.co/15x15/292d3e/292d3e.png) `#292d3e` background | ![#c792ea](https://placehold.co/15x15/c792ea/c792ea.png) `#c792ea` purple |
| ![#31364a](https://placehold.co/15x15/31364a/31364a.png) `#31364a` panels | ![#82aaff](https://placehold.co/15x15/82aaff/82aaff.png) `#82aaff` blue |
| ![#697098](https://placehold.co/15x15/697098/697098.png) `#697098` subdued | ![#c3e88d](https://placehold.co/15x15/c3e88d/c3e88d.png) `#c3e88d` green |

## Installing

Settings → Themes → Custom theme → paste the contents of
[`actual.css`](actual.css) into the CSS box, then Apply.

## About the palette

Every colour is quoted from `themes/palenight.json` of
[whizkydee/vscode-palenight-theme](https://github.com/whizkydee/vscode-palenight-theme),
and each declaration in `actual.css` carries the VS Code key it came from, so any
value can be traced back to its role in the original theme:

```css
--palenight-background-light: #31364a;    /* editorWidget.bg, tab.inactive  */
--palenight-selection: #2e3250;           /* peekViewResult.selectionBg     */
--palenight-comment-dim: #4c5374;         /* editorLineNumber.foreground    */
```

Two notes on choices that had no direct source:

- Palenight has no distinct pink. Where Actual's theme structure wants a second
  accent next to purple (selected sidebar items, hover states), this theme uses
  Palenight's blue `#82aaff`.
- Blue `#82aaff` and red `#ff5572` are the theme's UI values. The Palenight ANSI
  set used by terminal ports has `#82b1ff` and `#ff5370` instead; both pairs
  appear in the upstream theme file.

## Coverage

All **224** `--color-*` variables of Actual's built-in dark theme are defined, so
the theme does not fall back to the base theme anywhere — including the nine
`chartQual*` report colours.

## Credits

The original Palenight palette is by Olaolu Olawuyi
([whizkydee/vscode-palenight-theme](https://github.com/whizkydee/vscode-palenight-theme)),
published under the MIT license. This port only maps that palette onto Actual's
theme variables; the colours are theirs.

## License

MIT — see [LICENSE](LICENSE). Applies to this port.
