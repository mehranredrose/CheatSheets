# VSCode Cheat Sheet

Visual Studio Code is a powerful source code editor built by Microsoft. It offers a wide range of features for developers, including intelligent code completion, debugging, and version control integration. Below is a detailed cheat sheet to help you get started with VSCode.

## Basic Navigation

### Moving the Cursor
- **Arrow Keys**: Move up, down, left, and right.
- `Ctrl + f`: Forward one character.
- `Ctrl + b`: Backward one character.

### Word Movement
- `Ctrl + f`: Forward one word.
- `Ctrl + b`: Backward one word.
- `Ctrl + a`: Jump to the start of the line.
- `Ctrl + e`: Jump to the end of the line.

### Line Movement
- `Home`: Move to the beginning of the line.
- `End`: Move to the end of the line.
- `PgUp`: Move up one page.
- `PgDn`: Move down one page.
- `G`: Move to the last line.

## Editing Text

### Insert Mode
- **i**: Insert text before the cursor.
- **a**: Insert text after the cursor.
- **I**: Insert text at the start of the line.
- **A**: Insert text at the end of the line.
- **o**: Open a new line below the current line and enter insert mode.
- **O**: Open a new line above the current line and enter insert mode.

### Exiting Insert Mode
- **Esc**: Exit insert mode and return to normal mode.

### Cut, Copy, and Paste

- `x`: Delete the character under the cursor.
- `dd`: Delete the current line.
- `yy`: Yank (copy) the current line.
- `p`: Paste after the cursor position.
- `P`: Paste before the cursor position.
- `daw`: Delete a word.
- `yiw`: Yank a word.

### Search and Replace

- `/pattern`: Search for the pattern forward.
- `?pattern`: Search for the pattern backward.
- `n`: Move to the next occurrence of the search pattern.
- `N`: Move to the previous occurrence of the search pattern.

## Normal Mode Commands

### Basic Operations

#### Save and Quit
- **Ctrl + S**: Save the file.
- **Ctrl + Q**: Close the active editor tab.
- **Ctrl + W**: Close all editor tabs.

#### Undo and Redo
- `u`: Undo the last change.
- `Ctrl + y` or `Ctrl + Shift + Z`: Redo the last undone change.

### Navigation

- `gg`: Go to the first line of the file.
- `G`: Go to the last line of the file.
- `jk`: Move one character down and right.
- `hjkl`: Move one character up, down, left, and right respectively.

### Editing Text

#### Moving Between Lines
- `j`: Move down one line.
- `k`: Move up one line.
- `h`: Move left one character.
- `l`: Move right one character.
- `0`: Move to the start of the line.
- `$`: Move to the end of the line.

#### Editing Text
- `i`: Insert text before the cursor.
- `a`: Insert text after the cursor.
- `o`: Open a new line below the current line and enter insert mode.
- `O`: Open a new line above the current line and enter insert mode.
- `x`: Delete the character under the cursor.
- `dd`: Delete the current line.

### Advanced Operations

#### Multiple Commands
- Press `:` to start a command line, then type your commands separated by semicolons (`;`).
  ```bash
  :1,$s/foo/bar/g;
  ```

#### Macros
- Start recording a macro: `q` followed by a register letter (e.g., `qa`).
- Stop recording: `q`.
- Replay the macro: `@a`.

### File Management

- `Ctrl + O`: Open a file.
- `Ctrl + Shift + P`: Open Command Palette.

## Tips and Tricks

1. **Extensions**: Install extensions to enhance VSCode’s functionality. Search for extensions in the Extensions view (`Ctrl + Shift + X`).

2. **Keybindings**: Customize keybindings by editing the `keybindings.json` file.

3. **Settings**: Configure VSCode settings by editing the `settings.json` file or using the Settings UI (`Ctrl + ,`).

4. **Terminal**: Open a terminal in VSCode using `Ctrl + ` (backtick) to start coding in an integrated terminal.

5. **Debugging**: Use the debugging feature by pressing `F5` and configuring your launch settings in `.vscode/launch.json`.

6. **Version Control**: Integrate Git with VSCode for version control.

This cheat sheet provides a comprehensive overview of VSCode commands and operations. By mastering these elements, you can become more efficient in using VSCode for your development needs.

Happy coding with VSCode!
