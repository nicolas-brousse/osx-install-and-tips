---
layout: page
title: Sublime text
---

## Packages to install

```bash
$ apm install Sublime-Style-Column-Selection
$ apm install alignment editorconfig emmet color-picker
$ apm install language-docker language-haml language-mjml language-nginx
$ apm install markdown-preview pdf-view
$ apm install vim-mode yard
$ apm install monokai file-icons
# $ apm install vim-mode
```

## Configuration

```cson
"*":
  core:
    audioBeep: false
    disabledPackages: [
      "metrics"
    ]
    excludeVcsIgnoredPaths: false
    followSymlinks: true
    projectHome: "~/Projects"
    themes: [
      "one-dark-ui"
      "monokai"
    ]
  editor:
    backUpBeforeSaving: true
    fontSize: 10
    invisibles: {}
    preferredLineLength: 120
    showIndentGuide: true
    showInvisibles: true
    softWrap: true
    softWrapAtPreferredLineLength: true
  emmet: {}
  "file-icons":
    onChanges: true
  "one-dark-ui":
    layoutMode: "Compact"
  welcome:
    showOnStartup: false
```
