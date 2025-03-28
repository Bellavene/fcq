## Installation
Copy `fcq` file to your path

## Dependencies
[CopyQ](https://hluk.github.io/CopyQ/), [highlight](https://gitlab.com/saalen/highlight/), [ripgrep-all](https://github.com/phiresky/ripgrep-all)

## CopyQ integration / update on new entries
Create a command in CopyQ and paste this:
```
[Command]
Name=Update fzf
Automatic=true
Command="
    copyq:
    if ( isClipboard() )
      execute('curl', '-XPOST', 'localhost:6265', '-d', 'become:fcq')"
```
