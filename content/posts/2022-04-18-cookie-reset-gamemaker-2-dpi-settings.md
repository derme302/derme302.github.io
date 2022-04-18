---
title: "Cookie - Reset GameMaker 2 DPI Settings"
date: 2022-04-18T18:30:00+10:00
categories:
  - GameMaker
tags:
  - guide
---
GameMaker 2 has improved robustness of the UI significantly over GameMaker 1. However, I still ran into some issues today with the UI crashing after changing the DPI settings. It's annoying as you're unable to change the setting back as the UI crashes when you open it.

If you've run into the same issue, don't fear, it's pretty simple to fix.

Start by heading to the shared settings folder, on Windows that is:
```
C:\ProgramData\GameMakerStudio2
```
Or on MacOS:
```
/Users/Shared/GameMakerStudio2
```

Then open `dpi_override.json` and change it back to defaults by pasting this or modifying the values:
```json
[{"Key":"is_enabled","Value":false},{"Key":"value","Value":96}]
```

That should be it, hopefully GameMaker should open again without an issue.
