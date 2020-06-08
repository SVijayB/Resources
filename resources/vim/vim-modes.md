---
description: The different Vim Editor Modes
---

# Vim Modes

Once you have installed the Vim extension on VS Code, you can notice at the bottom of your IDE, the mode you are using. Namely Insert, Normal, Command, Visual and Replace Mode.

### Normal Mode

By Default, you will be on the normal mode on VS Code or your Vim Editor. You can access this mode by simply pressing the `Esc` key.

When in normal mode, one can traverse between lines of codes or text using various commands, we will discuss about these commands in the next section.

### Insert Mode

Insert mode, is the default mode in all the text editors. It's the mode in which when you press a key on the keyboard, it is inserted on your text editor.

To enter Insert mode, just press `i` when in normal mode or just press the `insert` button present on your keyboard. 

There are other command keys as well. 

* If you press the `a` key, the cursor moves after the current character and enters insert mode. 
* If you press the `o` key, a new line below the current line is created and you enter insert mode.
* The upper case `I (shift + i)`moves the cursor to the beginning of the line and enters insert mode.
* Upper case `A (shift + a)`moves the cursor to the end of the line and enters insert mode.
* Upper case `O (shift + o)`creates a new line above the current one and enters insert mode.

### Visual Mode

The Visual mode is used to select text or lines of code on the editor. It's like using your mouse to select text by clicking and dragging. When selected, you can copy, delete, replace and do other tasks on the selected lines.

To enter Visual mode, just press `v` on normal mode.

There are different sub-modes in Visual mode : 

* block-visual : Used to select a large scale or blocks of codes. To enter this mode, press `ctrl + v`.
* linewise-visual: This always select the complete line. You can enter this by pressing `shift + v`.

### Command mode

Command mode is like the normal mode but with a lot more features and command. To enter the command mode, press `: (shift + ;)`when in normal mode and then type the command. 

You can use `:h` or `:help` for more options and commands.

### Replace mode

The replace mode is used to type over the pre-existing code/text. To enter this mode, switch to normal mode and press `R (shift + r)`. Now whatever you type will replace the existing text. Every character you enter will replace the existing one.

### Documentation

You can learn more about Vim commands by going through Vim's documentations. You can find them [here](https://vimhelp.org/).

