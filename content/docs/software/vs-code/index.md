---
title: VS Code
---
VS Code is the IDE (Integrated Development Environment) we use at CHS. It is where we write all of our code in Engineering 3 and 4. (Engineering 1 and 2 use Arduino.)

## CircuitPython Setup

### Upload script

One of the best ways to test code is to upload it to the board and then the board will auto run it. This is done by using the launch configuration in the `.vscode` folder at the root of the directory. One prerequisite is that the extension [F5 anything](https://marketplace.visualstudio.com/items?itemName=discretegames.f5anything) must be installed.

```json
{
    "version": "0.2.0",
    "configurations": [
{
            
            "name": "Upload code to board",
            "type": "f5anything",
            "request": "launch",
            "command": "Copy-Item -Path \"${file}\" -Destination \"D:\\code.py\"",
            "showTerminal": false,
            "terminalName": "Code Uploader",
            
        }]
}
```
<!-- TODO: check if config is correct -->

the only change you might have to make is the name of the drive that is selected to copy to as that could be your `D:` drive as seen or any other such as `C:` or `E:`. to change  this just change the letter before `code.py` in the `"command":"` line.
