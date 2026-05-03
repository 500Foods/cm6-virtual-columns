# cm6-virtual-columns

A CodeMirror 6 plugin that implements virtual columns. This is when you can cursor up/down the editor and it doesn't move the column the cursor is in,
regardless of the length of content of that column. It adds spaces when needed to keep the cursor in the right column, and removes spaces from the ends
of lines when leaving, so it doesn't create any extra spaces when not needed.

## Motivation

Many years ago, this was a common thing in editors, particularly those from Borland. It makes it a lot easier to add aligned comments or code or other
text just by using the cursor keys, and without having to constantly look for your cursor when moving around the editor. There's an equivalent kind of
thing implemented in the `fake-virtual-space` plugin for Visual Studio Code.

These days, editors typically rely on the default cursor mechanism where it moves the cursor to the end of the line for shorter lines, but remembers the
position when you get back to a longer line, so long as you have only moved up/down and not left/right. So common that people probably don't even realize
that this isn't the only way to do things.

## Repository Information 
[![Count Lines of Code](https://github.com/500Foods/cm6-scroller/actions/workflows/main.yml/badge.svg)](https://github.com/500Foods/cm6-scroller/actions/workflows/main.yml)
<!--CLOC-START -->
```cloc
Last updated at 2026-05-03 23:36:12 UTC
-------------------------------------------------------------------------------
Language                     files          blank        comment           code
-------------------------------------------------------------------------------
Markdown                         2             10              2             46
YAML                             2              8             13             37
-------------------------------------------------------------------------------
SUM:                             4             18             15             83
-------------------------------------------------------------------------------
2 Files were skipped (duplicate, binary, or without source code):
  gitattributes: 1
  gitignore: 1
```
<!--CLOC-END-->

## Sponsor / Donate / Support
If you find this work interesting, helpful, or valuable, or that it has saved you time, money, or both, please consider directly supporting these efforts financially via [GitHub Sponsors](https://github.com/sponsors/500Foods) or donating via [Buy Me a Pizza](https://www.buymeacoffee.com/andrewsimard500). Also, check out these other [GitHub Repositories](https://github.com/500Foods?tab=repositories&q=&sort=stargazers) that may interest you.
