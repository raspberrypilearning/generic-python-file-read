To read a text file in Python you must `open` the file and then `read` its contents. 

When opening the file, use `with` and `as`.  This makes sure that, when your indented code has run, the file will automatically close. Closing files you don't need saves memory in your computer.

```python
with open(filename) as f:
```

Where `filename` is the name of the file you are opening, e.g. `'info.txt'`.

The file is loaded into the `f` variable, but not as text that Python can work with. To get the file as text, you need to use `read()`.

```python
with open(filename) as f:
  file_text = f.read()
  # Do something with the text
```