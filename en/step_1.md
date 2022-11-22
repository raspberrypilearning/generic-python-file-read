To read a text file in Python you must `open` the file and then `read` its contents. 

When opening the file, use `with` and `as`.  This makes sure that, when your indented code has run, the file will automatically close. Closing files you don't need saves memory in your computer.

```python
with open(filename) as f:
```

Where `filename` is the name of the file you are opening, e.g. `'info.txt'`.

Once you load your file, you can turn the whole file into a text string. Or, you can use a `for` loop to go through the file line-by-line.

### Turn the whole file into a text string
The file is loaded into the `f` variable, but not as a text string that Python can work with. To get the file as text, you need to use `read()`.

```python
with open(filename) as f:
  file_text = f.read()
  # Do something with the text
```

### Loop through the file, line by line
The file is loaded into the `f` variable. You can use a `for` loop to run the same code on each line of the file.

```python
with open(filename) as f:
  for file_line in f:
    # Do something with the line