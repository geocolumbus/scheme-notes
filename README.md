# Scheme Notes

## Install Scheme on Mac

Install from here:
http://ftp.gnu.org/gnu/mit-scheme/stable.pkg/10.1.9/

Link to the run time so you can run it in your terminal
```
ln -s /Applications/MIT\:GNU\ Scheme\ 10.1.9.app/Contents/Resources/mit-scheme /usr/local/bin/scheme
```

Add this to your path
```
export MITSCHEME_LIBRARY_PATH="/Applications/MIT\:GNU Scheme 10.1.9.app/Contents/Resources"
export PATH=$PATH:$MITSCHEME_LIBRARY_PATH
```

Run it
```
scheme -v

MIT/GNU Scheme microcode 15.3
Copyright (C) 2019 Massachusetts Institute of Technology
This is free software; see the source for copying conditions. There is NO warranty; not even for MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.

Image saved on Sunday June 9, 2019 at 1:18:03 PM
  Release 10.1.9 || Microcode 15.3 || Runtime 15.7 || SF 4.41 || LIAR/x86-64 4.118

Moriturus te saluto.
```

Start it as a REPL
```
scheme
```
How to exit the run time - press CTRL-Z

## Usage
```
git clone
cd scheme-notes
scheme --load hello
```