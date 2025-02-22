---
title: Bash shortcut
category: CLI
layout: 2017/sheet
tags: [Featured]
updated: 2023-10-23
keywords:
  - Shortcut
---

### Moving the cursor

| Expression | Description                                                     |
| ----------------- | -------------------------------------------------------- |
| Ctrl + a | Go to the beginning of the line (Home)                            | 
| Ctrl + e | Go to the End of the line (End)                                   |
| Ctrl + p | Previous command (Up arrow)                                       |
| Ctrl + n | Next command (Down arrow)                                         |
|  Alt + b  | Back (left) one word                                             |
|  Alt + f  | Forward (right) one word                                         |
| Ctrl + f  | Forward one character                                            |
| Ctrl + b  | Backward one character                                           |
| Ctrl + xx | Toggle between the start of line and current cursor position     |

### Editing

| Expression | Description                                                     |
| ----------------- | -------------------------------------------------------- |
| Ctrl + L |  Clear the Screen, similar to the clear command|
| Alt + Del | Delete the Word before the cursor.|
| Alt + d |  Delete the Word after the cursor.|
| Ctrl + d |  Delete character under the cursor|
| Ctrl + h |  Delete character before the cursor (Backspace)|
| Ctrl + w  | Cut the Word before the cursor to the clipboard.|
| Ctrl + k  | Cut the Line after the cursor to the clipboard.|
| Ctrl + u  | Cut/delete the Line before the cursor to the clipboard.|
| Alt + t  | Swap current word with previous|
| Ctrl + t |  Swap the last two characters before the cursor (typo).|
| Esc  + t |  Swap the last two words before the cursor.|
| Ctrl + y  | Paste the last thing to be cut (yank)|
| Alt + u  | UPPER capitalize every character from the cursor to the end of the current word.|
| Alt + l  | Lower the case of every character from the cursor to the end of the current word.|
| Alt + c  | Capitalize the character under the cursor and move to the end of the word.|
| Alt + r  | Cancel the changes and put back the line as it was in the history (revert).|
| Ctrl + _  | Undo|

### Process control

| Expression | Description                                                     |
| ----------------- | -------------------------------------------------------- |
|Ctrl + C |  Interrupt/Kill whatever you are running (SIGINT).|
|Ctrl + l |  Clear the screen.|
|Ctrl + s |  Stop output to the screen (for long running verbose commands). Then use PgUp/PgDn for navigation.|
|Ctrl + q |  Allow output to the screen (if previously stopped using command above).|
|Ctrl + D |  Send an EOF marker, unless disabled by an option, this will close the current shell (EXIT).|
|Ctrl + Z  | Send the signal SIGTSTP to the current task, which suspends it. To return to it later enter fg 'process name' (foreground).|