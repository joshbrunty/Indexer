# Indexer
Indexer is a Python script that generates an .html index of files within a selected directory. You can start from the current directory or from folder passed as first positional argument. Optionally filter by file types with --filter "\*.py". This script is an hodgepodge of older scripts [collected](https://stackoverflow.com/questions/10961378/how-to-generate-an-html-directory-list-using-python) & built over the years.

## Prerequisites:
* This script requires you to have **[Python > 3.x.x](https://www.python.org/downloads/)** installed on your system. 
* Ideally use the current build of **[Python 3.10](https://www.python.org/downloads/release/python-3100/)** (significantly faster processing on larger directories! 🏃)

## Usage
*python3 indexer.py /top_dir*

## Positional arguments:
* **top_dir**: top folder from which to start generating indexes (*uses current working directory/folder if not specified*).

## Optional arguments:
* ***-h, --help***: show this help message and exit.
* ***-f, --filter***: only include files matching [glob](https://docs.python.org/3/library/glob.html) (*i.e. indexer.py --filter '\**/*.jpg'*).
* ***-o filename, --output-file filename***: Custom output file (by default generates "index.html")
* ***-r, --recursive***: recursively process nested folders/directories (*Off/False by default*).
* ***-v, --verbose***: verbosely list every processed file. (*NOTE: will take longer time with complex file tree structures on slow terminals.*)

## Features: 
* File Size & Modified Time display for each file. 
* Create a custom output file (*by default *index.html* is generated*).
* Ability to match specified parameters using [glob](https://docs.python.org/3/library/glob.html) (*'\**/*.jpg' & '\**/*.UFD'*).
