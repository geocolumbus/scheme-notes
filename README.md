# Scheme Notes

## Install Scheme on MacOS

Scheme is available here (if scheme has a more modern version, just change out the version number in these instructions)
http://ftp.gnu.org/gnu/mit-scheme/stable.pkg/10.1.9/

You want to run the DMG installer on your Mac.
```
mit-scheme-10.1.9-x86-64.dmg
```

Now that it is installed in your Application folder, we want to link to the run time so we can run it from the terminal.
```
ln -s /Applications/MIT\:GNU\ Scheme\ 10.1.9.app/Contents/Resources/mit-scheme /usr/local/bin/scheme
```

Add this to your ```~/.bash_profile```
```
export MITSCHEME_LIBRARY_PATH="/Applications/MIT\:GNU Scheme 10.1.9.app/Contents/Resources"
export PATH=$PATH:$MITSCHEME_LIBRARY_PATH
```

Restart your shell and try running it
```
scheme -v
```

You should see:
```
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
To exit the REPL - press CTRL-Z

## Usage
```
git clone
cd scheme-notes
scheme --load hello
```

## Reference

* [MIT Scheme Page](https://www.gnu.org/software/mit-scheme/)
* [Scheme Reference Manual](https://www.gnu.org/software/mit-scheme/documentation/mit-scheme-ref/index.html)
* [Scheme Users Manual](https://www.gnu.org/software/mit-scheme/documentation/mit-scheme-user/index.html)
