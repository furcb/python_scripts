# Python Scripts

A collection of scripts which handle a variety of task on linux machines.

## Downloader

Generic file/document downloader that uses CSS Selectors to identify and retrieve said information.
Downloader also uses pythons multiprocessing module for concurrent download.

### Usage

```sh
downloader links_file.txt	# Downloads files from links specified in links_file.txt
downloader -n links_file.txt 	# Downloads pages and tries to get information using CSS selector.
```

## Journal Entry

Journal Entry or jot, is a journal entry generating script. It can list, create, and open entries.

### Usage

```sh
jot # Creates a new entry and opens it using the current date.
jot 20190912 # Attempts to open the journal entry for 20190912, if none exists it creates a new one.
```

## New Script

New Script or ns, is a script generating program. It uses a simple template system to create script
files based on a keyword (generally the script language).

### Usage

```sh
ns green 	# Creates a script called green with the default template boilerplate.
ns py blue	# Creates a script called open, and fills it with the boilerplate from py.
```

## Sort Files

Sort files, uses Linux's link system to organize files into directories based on criteria given.

### Usage

```sh
sort_files path/to/files	# Sorts files in path/to/files using only the date based criteria

sort_files -o path/to/output_dir path/to/files warm 	# Sorts files into another directory using
							 # "warm" and dates as criteria. Output
							 # directory is useful for SMB/Cifs
							 # directories that do not support Linux
							 # links.
```
