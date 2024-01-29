<h1 align="center">CTICF Filetype</h1>
<p align="center"><strong>Our file format CTICF (Console Text Indexing & Coloring Format), specifically made for Python Console Applications to manage their text UI in one singular file, and also add color to it.</strong></p>

This format was made specifically for [BastionCMD](https://www.github.com/BastionMC/BastionCMD), but you can use it in any of your own programs! It's in plain-text, so you don't need to worry about writing the files in any special programs.

<h1 align="center"><img image-rendering="pixelated" height="24px" width="24px" src="graphics/Installation.png">Installation</h1>

1. Select the `cticf.py` file from the source of the latest release.
2. Put the file in the same folder as your main Python file.
3. Import `cticf`:
```py
import cticf
```
6. **You're done, the setup process is complete.**

<h1 align="center"><img image-rendering="pixelated" height="24px" width="24px" src="graphics/How_to_use.png">How to use</h1>
Here's how you can write in this format, and how to use it. Almost everything you want to know is explained here.

---

**Formatting Characters**

The formatting characters consist of the dollar sign, `$`, and the paragraph symbol, `§`. A combination of the two symbols is used for every formatting character combination. Here's all the combinations that you can use:

1. $$ - This combination is used as an insertion point for text. It does not have any arguments.
2. §§ - This combination is used for changing the text color. It has three arguments: the color, the brightness, and the ground. The color can be `r|g|y|b|m|c|w|0`, standing for red, green, yellow, blue, magenta, cyan, white & black. The brightness can be set to `d|n|b` (meaning dim, normal & bright). The ground is either the foreground or the background, so that's `f|b`.
3. §$ - Reset's the text color back to the terminals default text color, if needed.
4. $§ - Different strings get split at this character.
   
---

**Comments**

Guess what? You can comment the beginning of files! Just write a `#` in it's own seperate line to indicate that the actual file stuff starts from there.
 
---

**Reading a file**

Once you imported CTICF, reading a file is really easy. You can simply read a file with the following code:

```py
import cticf

ui_strings = cticf.rfile("path/to/file.cticf")
ui_string = ui_strings[0]

print(ui_string)
```

This function will return a list with all of your formated strings. You can just print the strings, and they should be formatted. If you want to insert text, the following how-to might be helpful to you:

---

**Inserting text**

After you've read a file, you can insert text into one of the indexed strings, and print that string to the console:

```py
import cticf

ui_strings = cticf.rfile("path/to/file.cticf")
ui_string = ui_strings[0]
ui_string = cticf.inserts(ui_string, "Hello World!")

print(ui_string)
```

