# codes2pdf
Auto generate a PDF notebook from your source codes (useful for your ACM-ICPC cheatsheet)

## Dependencies

This generator works in both Linux and Windows, so check how to install TeX Live in your OS.

TeX Live for linux:

    sudo aptitude install texlive

TeX Live for Windows:

    download installer (install-tl-windows.exe) from https://www.tug.org/texlive/acquire-netinstall.html
    
    
Also install Node.js and NPM on your machine (you can download them from https://nodejs.org/en/download/).

After installing Node.js on Linux, add this command to your ~/.bashrc:

    export PATH="$HOME/.npm_modules/bin:$PATH"


## Install

    Download This Repository and Unzip it.     
    sudo npm install -g ./codes2pdf

## Update

    sudo npm install --update -g ./codes2pdf

## Use

    Usage: codes2pdf <source_dir> [options]

    Auto generate a PDF notebook from your source codes

    Options:

        -V, --version             output the version number
        -a --author [name]        author's name to be added in the notebook
        -i --initials [initials]  initials of the author to be placed in the upper-right corner of all pages
        -o --output [filename]    output file for the notebook. Default to `./notebook.pdf`
        -h, --help                output usage information


example:

    codes2pdf <adress to codeFolder> --author <author name> --initials <team or college initials> --output <o/p file name>

The notebook generator will add your source code with syntax highlighting, additionally
you can add .tex files which will be rendered as Latex code.

## Notes

- Only for 1 level in source code.
- Use spaces insead of underscore (in the filenames) to print a prettier TOC.
- The generated notebook will have three columns in each page.
