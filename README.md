pyscripts
=========

This is supposed to be a collection of python scripts for usefule everyday use.

Copyright (c) 2015 by Stefan Lehmann

License: MIT License

dupy.py - Duplicate finder
--------------------------
Find duplicate files within directories. The file comparison is done by Pythons
[`filecmp.cmp()`](https://docs.python.org/2/library/filecmp.html#module-filecmp)
function.

### Features

* recursively search a parent directory for duplicate files
* choose which dupes to keep and which to delete
* filter filetypes


```bash
usage: dupy.py [-h] [-t FILETYPES] [-l] [-r] [-v] [-s] directory

Find duplicate files.

positional arguments:
  directory             directory to find duplicates

optional arguments:
  -h, --help            show this help message and exit
  -t FILETYPES, --filetypes FILETYPES
                        only list file with these endings, separated by comma
                        (e.g.: mp3,m4a)
  -l, --list            only list dupes
  -r                    recursively search all subdirectories
  -v, --verbose         verbose output
  -s, --shallow         use shallow file comparison (may be faster, but less
                        relyable)
```
