FATI are two modules for AT-commands
connection over USB and by TCP using SSH
to run CLI commands and return stdout scope

# Examples using CMD module (Inside ADB CLI commands)

To run an example for a 'date' command over USB (by using ADB):
```
from myadblib import CMD

command = 'date'
output = ADB.run(command)
```  
  by default ABD.run() has a param called print_result=True

Same last example
```
from myadblib import ADB

command = 'date'
output = ADB.run(command, print_result=False)
``` 
  for lines in output:
    print(lines)
