---
description: All the Vim commands needed to get started
---

# Vim Commands

If you haven't already tried vimtutor, you should do so. It helps you learn all the basic commands needed to get started with Vim. But if you choose not to, I have mentioned all the commands needed below. 

### Cursor Movement

* **j** to go one row down 
* **k** to go one row up 
* **l** to go one character right
* **h** to go one character left

You can add a number at the beginning of these commands, like `4j`or `5l`.This would execute the command by the number mentioned. That is, 4j would move the cursor 4 rows down. and 5l would move the cursor 5 characters to the right.

### Moving between words

* **w** moves the cursor to the beginning of the next word.
* **e** moves the the cursor to the end of the word.
* **b** moves the cursor to the beginning of the previous word.

**Note** : You can execute the same command multiple times by adding a number at the beginning. Using the Upper case of each of these commands also work. They go to the word mentioned before or after a white-space.  

### Moving between lines

* Press **0** to move to the beginning of the line.
* Pressing **$ \(Shift + 4\)** moves to the end of the line.
* Press the  **^ \(Shift + 6\)** to move to the first character of the line.
* You can also move to the corresponding brackets by using **% \(Shift + 5\)**

### Finding Occurrences

* Use **f** to go to the first occurrence of a character. That is, If you press **f**   followed by a word, or a character, the cursor moves to that position.
* Using **F \(Shift + f\)** goes to the first occurrence of a character backwards. 
* To search for a word, occurrence just use `/(type the word here)` and then press enter. This, takes you to the first occurrence. Now, press **n** to go to the next occurrence. You can also use  **N \(Shift + n\)** to move to the previous occurrence. 
* To search backwards \(From the end of the file\), use **? \(Shift + /\)**.
* When searching backwards, the roles of **n** and **N** are opposite.

### Copy, Paste, Delete and Undo

* To copy a line, just press **y** twice. 
* To paste, press **p**
* To paste on top of the current line, press **P \(Shift + p\)**.
* To delete, press **d** twice. 

 **Note** : The delete line is automatically copied to your clipboard. 

### Selection Mode Commands

* First enter visual mode by pressing **v**.
* In visual mode, you can change indentation by using the **&lt; \(Shift + ,\)** or the &gt; **\(Shift + .\) .**
* You can switch between upper and lower case by using **~ \(Shift + \`\)** 
* You can mark the nearest block with parenthesis by first pressing **a** and then followed by **b**.
* You can also mark the nearest block within brackets by first pressing **a** followed by **B \(Shift + b\)**
* If you replace the **a** with **i** in the above two commands, you can select only the contents within the brackets/parenthesis \(without the brackets\). 

**Note** : You can use `.` to repeat the latest command.

There are several methods to learn Vim commands easily. However, there is a more fun and intuitive method, there is a game called the Vim adventures that lets you learn Vim commands easily. Click [here ](https://vim-adventures.com/)to play Vim adventures. 



