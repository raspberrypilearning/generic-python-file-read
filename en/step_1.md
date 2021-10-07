To read a text file in Python you must `open` the file and then `read` its contents. 

When opening the file, use `with` and `as` — this pair of keywords means that the indented code under the `with… as` line has run, the file will automatically close. This saves memory in your computer.

```python
with open(filename) as file:
```

Where `filename` is the name of the file you are opening, e.g. `'info.txt'`.

To read the file's contents, use `read()`:

```python
with open(filename) as file:
  contents = file.read()
  # Do something with the contents
```