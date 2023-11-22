# TeXnoCrat

This is a quickstart $\LaTeX$ setup.

## Features

### Report Class

The `report` document class is used, giving: parts, chapters, sections, and subsections.
If you don't like or need "parts", just don't use it.

### Environments
 
There are environments for:

* definitions
* examples
* notes
* lemmas
* theorems
* proofs

See the example for syntax.
The colors can be changes in `envs.sty`.

### Bibliography

Add entries to the bibliography with `\cite{mycitation}`, and add `mycitation` to `notes.bib`.

You can append new citations to `notes.bib` with the `bibsearch` tool from this repo
Run
```bash
./bibsearch --help
```
for usage.

### Index

To add items to the index, say for "widget", place `\index{widget}` in the appropriate location.

### Font Awesome

Font awesome commands are available,
such as the pencil icon used by the custom `todo` command in `commands.sty`.
See [here](http://mirrors.ctan.org/fonts/fontawesome/doc/fontawesome.pdf) for a list of the commands.

### Name change

You can change the name of the main tex file (currently `notes.tex`),
but make sure to edit line 9 of `Makefile`.

### Making it your own

Edit `body.tex`.

### Building

You will need several latex packages installed, but once that is done you can build with:

```bash
make
```

#### cleaning build files

```bash
make clean
```
