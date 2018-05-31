---
date: 2016-02-17 18:47
category: news
---

Fountain Mode version 2.0 is [now available][1].

## Exporting
- Export to LaTeX, HTML, Final Draft, Fountain or your very own custom formats
- Huh? Why export Fountain? See #33
- Separation of the [LaTeX template](https://www.sharelatex.com/project/54ed9180966959cb7fdbde8e) project and the [HTML template](https://github.com/rnkn/mcqueen) project
- Skip the Lisp export entirely and use `fountain-export-shell command` with ['afterwriting](https://github.com/ifrost/afterwriting-labs/blob/master/docs/clients.md) or [TextPlay](https://github.com/olivertaylor/Textplay) or whatever you like
- New parsing engine reads Fountain text into Lisp data for further magic
- New export engine allows much faster export—to virtually any format
- Choice of export to standalone document or a snippet
- ~~Template replace function system allows adding your own keys to templates, e.g. add `("email" (lambda nil user-mail-address))` to `fountain-additional-template-replace-functions` and all instances of `${email}` in template will be replaced with your email~~
- All export templates are totally customizable

## Not just screenplays
- Auto-align elements to different columns for different formats (e.g. `screenplay` or `stageplay`), just include `format: stageplay` or whatever in your metadata
- Action is now a first-class element that can be auto-aligned (like, for stageplays)

_n.b. the export templates are really geared towards screenplays, so if you're a playwright and feel lost please get in touch and we'll see what we can do_

## New abilities
- Scene numbers optionally align to the right margin
- `fountain-upcase-line` with <kbd>C-c C-c</kbd> (`fountain-continued-dialog-refresh` is moved to <kbd>C-c C-d</kbd>)
- Prefix `fountain-upcase-line` or `fountain-upcase-line-and-newline` with <kbd>C-u</kbd> to make insert `.` at the beginning to make a forced scene heading
- Terminal-friendly key map
- Align the title page contact info to the left or right

## Better existing abilities
- `imenu` regular expression now show section heading prefixes (e.g. `# act II` instead of `act II`)
- `fountain-mark-scene` now excludes marking a following outline heading
- For those writers who like to include blank lines _within_ dialogue, you should be golden
- It should now be impossible to get into an endless loop

## Removing the cruft
- Removed reliance on Prince for PDF export (use LaTeX instead)
- Reduced reliance on `s.el` ~~(soon to be removed as dependancy)~~ (now removed as dependency)
- Removed `fountain-uuid` and related variables
- Title page templates now only use a single contact box instead of a left and right

## Notes on upgrading

As this is a major version upgrade, some backwards compatibility is lost. I've tried to document this as much as possible here: [Upgrading From 1.x to 2.0](https://github.com/rnkn/fountain-mode/wiki/Upgrading-From-1.x-to-2.0). If you have any trouble, please [raise an issue](https://github.com/rnkn/fountain-mode/issues).


[1]: https://github.com/rnkn/fountain-mode/releases/v2.0.0
