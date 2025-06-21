#!/bin/bash
/opt/homebrew/bin/wine "/Users/ali/.wine/drive_c/users/ali/AppData/Local/Programs/Python/Python310/python.exe" "$@"



to use python inside wine as a interpreter in IDEs we need to make a wine-python.sh file with the following content^ and then use that path as an interpreter, also don't forget to chmod add permissions to execute.
