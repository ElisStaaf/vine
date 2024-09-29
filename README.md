# QV
QV - Quantum Visual editor, is a fast and intuitive terminal-based text editor based on the [kilo](https://github.com/snaptoken/kilo-src) editor, with a _lot_ of improvements! For example: better syntax highlighting! Cool, right?

Install
-------
To install, simply:
```bash
git clone --depth 1 https://github.com/ElisStaaf/qv ~/qv
```
And then, you have two options: if you're on a system that supports `.sh` files, you're in luck!  
  
**Init via init.sh**
```bash
bash ~/qv/init.sh
```
This will check that everything is okay, and then will install a shortcut to run the executable.
_But_, you can do everything, all on your own:  
  
**Init from scratch via linux BASH**
```bash
echo "alias qv=\"~/qv/build/qv.exe\"" >> ~/.bashrc
```  
  
**Init from scratch via windows**
```pwsh
"function qv {
    ~/qv/build/qv.exe
}" >> $env:USERPROFILE/Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
```

Get Started
--------
To get started, just open a file via QV!
```bash
qv <filename>
```
Currently, QV includes syntax highlighting for the following languages:  
-  C/C++
-  Shell
-  Golang
-  Python
-  JS/TS
-  C#
  
But you can ofcourse modify the source-code to add more! I shall for this tutorial
use the "C" programming language.
```bash
touch "main.c" # Create file
qv "main.c" # Open file
```
I am greeted to this interface:
[![File could not be loaded.](https://github.com/ElisStaaf/qv/blob/main/startup.png?raw=true)](https://github.com/ElisStaaf/qv/startup.png)
Great! It started up! I'm writing a simple Hello World app, so i can just write this: