# notebook-generator
(Auto) generate notebooks from your source code. Useful for ACM-ICPC

## Dependencies

This generator works in both linux and windows, so check how to install texlive in your OS.

texlive for linux:

    aptitude install texlive

texlive for windows:

    download installer (install-tl-windows.exe) from https://www.tug.org/texlive/acquire-netinstall.html

## Install

    npm install -g notebook-generator

## Use

    Usage: notebook-generator <soruce_dir> [options]

    Auto generate notebooks from your source code

    Options:

        -V, --version             output the version number
        -a --author [name]        author's name to be added in the notebook
        -i --initials [initials]  initials of the author to be placed in the upper-right corner of all pages
        -o --output [filename]    output file for the notebook. Default to `./notebook.pdf`
        -h, --help                output usage information


example:

    notebook-generator ./ /tmp/team_reference.pdf
    notebook-generator ./ --author "Universidad Tecnologica de Pereira" --initials UTP

The second one will create a 'notebook.pdf' file in the current directory.

## Example PDF

Here you can find an example https://github.com/pin3da/Programming-contest/blob/master/codes/notebook.pdf

## Files

The notebook generator will add your source code with syntax highlight, additionally
you can add .tex files which will be rendered as latex code.

## Notes:

- Try to use up to 3 "levels" in your source code.
- Use spaces insead of underscore (in the filenames) to print a prettier TOC.

----
[Manuel Pineda](https://github.com/pin3da/)
