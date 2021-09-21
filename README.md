[![](https://vsmarketplacebadge.apphb.com/version/tcneuen.blamer-vs.svg)](https://marketplace.visualstudio.com/items?itemName=tcneuen.blamer-vs)
[![](https://vsmarketplacebadge.apphb.com/installs/tcneuen.blamer-vs.svg)](https://marketplace.visualstudio.com/items?itemName=tcneuen.blamer-vs)

# SVN Gutter (fork/tcneuen)

This is the Visual Studio Code version of the [Blamer](https://github.com/BeauAgst/Blamer) plugin, built for Sublime Text and a published fork of the [original from BeauAgst](https://github.com/BeauAgst/blamer-vs) due to inactivity.

[Pull requests are always welcome!](https://github.com/tcneuen/blamer-vs/issues/)

## Commands:

This extension contributes the following commands to the Command palette.

`SVN Gutter - Show Blame`: Adds icons to gutter with tooltips containing information from each revision

`SVN Gutter - Clear Blame`: Clears icons and tooltips

## Shortcuts:

Currently only a single keyboard shortcut is available.

**SVN Gutter - Show Blame**
`CTRL + ALT + D` (Windows)
`CTRL + CMD + X` (Mac)

## Features

When run, this extension will place an icon next to each line of your file. Each differently-coloured icon means a different revision. Hovering a line will produce a tooltip, showing the committer, date, and message.

For example if you're working on a project and you want to see who modified a specific line:

![Example Usage](example.gif)

## Requirements

This extension requires that you're either:

- On a Windows machine with Tortoise SVN installed, with command-line tools.
- A Unix machine.

## Extension Settings

**Enable Detail** - By default, the extension get detailed log information for each unique revisions. Disabling this can increase speed, while still showing revision, date, & author in the tooltip.

**Enable Pips** - By default, the extension displays a coloured pip next to each line number. This can be turned off, whilst still showing the blame information in the tooltip.

## Known Issues

### From upstream

- When detail is enabled, can be slow, because all unique logs have to be retrieved first. ([#3](https://github.com/BeauAgst/blamer-vs/issues/3))
- Authentication errors [#5](https://github.com/BeauAgst/blamer-vs/issues/5), [#9](https://github.com/BeauAgst/blamer-vs/issues/9)

## Future features

- Automatic blame on file open
- Ideas and contributions always welcome!

## Release Notes

## 0.5.2

- Add a new option to disable fetching details via svn log
- Percentage complete when pulling logs
- Fallback on blame info when log fails instead of failing completely
- Dependency updates

## 0.5.1

- Handle cases where author metadata is missing [#53](https://github.com/BeauAgst/blamer-vs/issues/53)
- Use spawn instead of exec [#53](https://github.com/BeauAgst/blamer-vs/issues/53)
- Dependency updates

## 0.5.0

- Mac blame shortcut added
- Setting added to disable visual pips [#10](https://github.com/BeauAgst/blamer-vs/issues/10)
- Better error handling, blame indicator in workbench [#3](https://github.com/BeauAgst/blamer-vs/issues/3)

## 0.4.0

- Revision number added to tooltips [#7](https://github.com/BeauAgst/blamer-vs/issues/7)

## 0.3.2

- Fixed decoration issue causing characters to show incorrectly dependant on the language [#6](https://github.com/BeauAgst/blamer-vs/issues/6)

## 0.3.1

- Removed formatting error in decoration caused by conflict with `mailto:`
- Added icon to extension

## 0.3.0

- Linux support added. [#2](https://github.com/BeauAgst/blamer-vs/issues/2)

## 0.2.0

- Added keyboard shortcut
- Fixed readme typo

## 0.1.0

- Initial release
