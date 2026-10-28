# TextToFlow

Type plain-English steps, get a flowchart or org chart. One HTML file. No install, works offline.

**Open it here: https://suhailasrulsani-git.github.io/texttoflow/**

**Watch the demo (1:52, sound on): https://suhailasrulsani-git.github.io/texttoflow/TextToFlow-demo.mp4**

Your diagrams stay in your own browser. Nothing is sent anywhere.

## How to use

Use the link above, or to keep a copy:

1. Download `TextToFlow.html`.
2. Double-click it. It opens in Edge or Chrome.
3. Type one instruction per line on the left. The diagram draws itself on the right.

You can also drag, link, rename and delete boxes on the diagram. The text updates to match.

## Flowchart

```
Start, go to Read file
Read file, go to Check user
if user found, go to Send email
else go to Log error
Is admin?, if yes, go to Admin page
Send email, go to End
```

- `if ...` / `else ...` makes a diamond with Yes / No arrows
- A name ending in `?` is a diamond too
- `go to X` on its own carries on from the last box
- Lines starting with `#` are ignored

## Org chart

```
Sara (Head of IT) reports to Tom (CEO)
Ali (Engineer) reports to Sara
Ben (Analyst) reports to Sara
```

Job title only needed once.

## Loops, notes, lanes

```
for each server, go to Check disk space
Check disk space, if disk full, go to Clean temp files
else go to next server
Clean temp files, go to next server
when done, go to Send report
note Send report: goes to the IT Ops mailbox
lane Service desk: Check disk space, Clean temp files
```

## Checklists (to-do list step)

```
Start, go to Set up laptop
todo Set up laptop: Install apps, [x] Encrypt disk, Set up MFA
Set up laptop, go to End
```

- One box with a tick box per item, plus a count like 1/3
- `[x]` = done. Click a tick box on the diagram to tick it - the text updates too
- Every item ticked = the box turns green
- Right-click a checklist > Add item, or drag "Checklist" from the bar

## Shapes are picked for you

| Shape | When |
|-------|------|
| Rounded | Start, End, Stop, Finish, the first box, any box with no arrow out |
| Diamond | `if ...`, or a name ending in `?` |
| Cylinder (database) | name has DB, Database or SQL |
| Hexagon (loop) | `for each ...` |
| Checklist | `todo Name: item, item` |
| Slanted | name starts with Read, Get, Send, Save, Print or Export |
| Rectangle | everything else |

- Red box: name has error, failed, exception, invalid, denied, timeout...
- Green box: name has success, completed, done, OK, passed...
- Yes arrows are green, No arrows are red
- Right-click a box to pick a shape yourself

## Features

- Top-down or left-right layout, auto layout, zoom and pan
- Undo / redo (Ctrl+Z / Ctrl+Y)
- Save and open your own `.texttoflow` file (Ctrl+S / Ctrl+O). Open also takes a `.txt` of instructions
- Export PNG, SVG or draw.io (`.drawio`)
- Copy picture - paste straight into Outlook, Teams or Word
- Step numbers (1 2 3 button)
- Light / dark theme
- 10 examples in the Examples menu
- Remembers your last diagram in the browser
- Built-in help (the `?` button)

## Browsers

Tested in Chrome and Edge. Firefox and Safari should work, but Save / Open fall back to Downloads and a file picker there.
