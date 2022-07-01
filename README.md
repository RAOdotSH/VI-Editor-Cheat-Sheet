<!-- [] Language: markdown
[] Path: vi.md
[] Title: **Vi Editor Cheat Sheet**
[] Tags: vi, editor, vim, vi-editor
[] Date: 07-01-2022
[] Type: cheat-sheet
[] Category: cheat-sheets
[] Visibility: public 
 -->
## To start the **Vi editor**
```bash
vim
```

## To open a file
```bash
vim {filename}
```

## Modes of the **Vi editor**
### Basically there are two modes in the **Vi**
    - **Visual/Normal Mode** -> Default mode where you can only view the contents of the file.
    - **Insert Mode** -> In this mode you can edit the contents of the file.

## Command execution in the **Vi editor**
### Commands can be executed using vi or ex command.
    - vi command -> `vi` -> Executed immediately based on sequential keystrokes.
    - ex command -> `ex` -> These commands begin wiht `: [command]` and are executed when pressed `Enter`.

# Vi Editor Commands
---
## Global
---
| **Sr. No.** | **Command** | **Description** |
| :---------: | :---------: | :-------------: |
| **1** | <kbd>ESC</kbd> | Escape to command mode |
| **2** | <kbd>:</kbd> | Enter command mode |
| **3** | <kbd>/</kbd> | Search |
| **4** | <kbd>u</kbd> | Undo previous command |
| **5** | <kbd>Ctrl+r</kbd> | Redo previous command |
| **6** | <lbd>.</kbd> | Repeat last command |
| **7** | <kbd>Ctrl+w</kbd> | Delete word |
| **8** | <kbd>Ctrl+u</kbd> | Delete line |
| **9** | <kbd>Ctrl+x</kbd> | Exit |
| **10** | <kbd>Ctrl+y</kbd> | Paste |
| **11** | <kbd>Ctrl+z</kbd> | Suspend |
| **12** | <kbd>Ctrl+c</kbd> | Cancel |
| **13** | <kbd>Ctrl+a</kbd> | Start of line |
| **14** | <kbd>Ctrl+e</kbd> | End of line |
| **15** | <kbd>:w</kbd> | Save |
| **16** | <kbd>:q</kbd> | Quit |
| **17** | <kbd>:wq</kbd> | Save and quit |
| **18** | <kbd>:w!</kbd> | Save as |
| **19** | <kbd>:q!</kbd> | Quit without saving |
| **20** | <kbd>:wq!</kbd> | Save as and quit |
---

## Editing
---
| **Sr. No** | **Shortcut** | **Description** | **Aliases** |
| :--------: | :-------: | :-------------------------: | :-------: |
| **1** | <kbd>Insert</kbd> | Toggles INSERT/REPLACE mode | None |
| **2** | <kbd>i</kbd> |  INSERT before the cursor | None |
| **3** | <kbd>I</kbd> | INSERT at beginning of line | None |
| **4** | <kbd>a</kbd> | INSERT after the cursor | None |
| **5** | <kbd>A</kbd> | INSERT at end of line | None |
| **6** | <kbd>s</kbd> | Delete the character at the cursor (enters INSERT Mode) | None |
| **7** | <kbd>S</kbd> | Delete the the line (enters INSERT Mode) | None |
| **8** | <kbd>r</kbd> | REPLACE the character at the cursor | None |
| **9** | <kbd>R</kbd> | REPLACE the the line | None |
| **10** | <kbd>Delete</kbd> | Delete the character at the cursor | <kbd>x</kbd> |
| **11** | <kbd>Backspace</kbd> | Delete the character before the cursor | <kbd>x</kbd> |
| **12** | <kbd>dd</kbd> | Delete the line | <kbd>d</kbd> |
| **13** | <kbd>dw</kbd> | Delete the word | None |
| **14** | <kbd>{num}dd</kbd> | Delete {num} of lines | None |
---

### Note:
```bash
INSERT -> Insert Mode - You can insert text at the cursor position.
REPLACE -> Replace Mode - You can replace the text at the cursor position.
```
---
## Cursor Movement
---
| **Sr. No** | **Shortcut** | **Description** | **Aliases** |
| :--------: | :-------: | :-------------------------: | :-------: |
| **1** | <kbd>h</kbd> | Move the cursor left | kbd>&leftarrow;</kbd> |
| **2** | <kbd>j</kbd> | Move the cursor down | kbd>&downarrow;</kbd> |
| **3** | <kbd>k</kbd> | Move the cursor up | kbd>&uparrow;</kbd> |
| **4** | <kbd>l</kbd> | Move the cursor right | kbd>&rightarrow;</kbd> |
| **5** | <kbd>w</kbd> | Jump to start of next **word** | None |
| **6** | <kbd>W</kbd> | Jump to start of next **WORD** | None |
| **7** | <kbd>e</kbd> | Jump to end of the next **word** | None |
| **8** | <kbd>E</kbd> | Jump to end of the next **WORD** | None |
| **9** | <kbd>b</kbd> | Jump to start of previous **word** | None |
| **10** | <kbd>B</kbd> | Jump to start of previous **WORD** | None |
---

### Note:
```md
<kbd>Space</kbd> and <kbd>Backspace</kbd> can also be used to navigate left and right in command mode.
---
**word** -> A word is a sequence of letters, digits, and underscores.
**WORD** -> A WORD is a sequence of letters, digits, underscores and punctuation.
```
---

## Searching
---
| **Sr. No** | **Shortcut** | **Description** | **Aliases** |
| :--------: | :-------: | :-------------------------: | :-------: |
| **1** | <kbd>/</kbd> | Search for the next occurrence of the character at the cursor | None |
| **2** | <kbd>?</kbd> | Search for the previous occurrence of the character at the cursor | None |
| **3** | <kbd>n</kbd> | Search for the next occurrence of the character under the cursor | None |
| **4** | <kbd>N</kbd> | Search for the previous occurrence of the character under the cursor | None |
| **5** | <kbd>/{text}</kbd> | Search for the next occurrence of the text | None |
---

## Navigation
---
| **Sr. No** | **Shortcut** | **Description** | **Aliases** |
| :--------: | :-------: | :-------------------------: | :-------: |
| **1** | <kbd>0</kbd> | Go to first character of the line | None |
| **2** | <kbd>$</kbd> | Go to last character of the line | None |
| **3** | <kbd>^</kbd> | Go to the non blank character of the line | None |
| **4** | <kbd>G</kbd> | Go to the last line | None |
| **5** | <kbd>n</kbd><kbd>GM</kbd> | Go to line n | None |
---

## Misc
---
| **Sr. No** | **Shortcut** | **Description** | **Aliases** |
| :--------: | :-------: | :-------------------------: | :-------: |
| **1** | <kbd>j</kbd> | Join the next line with the current line | None |
| **2** | <kbd>c</kbd> | Delete character from the cursor position (enters INSERT Mode) | None |
| **3** | <kbd>:e</kbd> | Reload current file | None |
