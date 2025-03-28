## Installation
Copy `fcq` file to your path

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
