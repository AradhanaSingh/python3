

### Lesson 1:  

* If you forgot to save output in a variable you can use underscore _ to get the the reusult of the last operation that you performed . only available in interactive mode.
* For hlep : example help(print)
* To quit  : quit()  or CTRL+D 

Add nextbus.py

```python
# Creating a File  with some modification to take input 

import sys

print('Commond options:', sys.argv) # Will allow to pass differnet arguments in the command line
raise SystemExit(0) # To make program quit 

import urllib.request # Allows to make http call to feth website 
u = urllib.request.urlopen('http://ctabustracker.com/bustime/map/getStopPredictions.jsp?stop=14787&route=22')
data = u.read()

from xml.etree.ElementTree import XML
doc =XML(data)

for pt in doc.findall('.//pt'):
    print(pt.text)
    
```



```Python
# nextbus.py

import sys
if len(sys.argv) !=3:
    
print('Command options:, Sys.argv)
import urllib.request

```



Python debugging
===============

1. python3 -i filename [input_parameters]
Runs the program and drops you at interactive prompt after the error. Values can be checked in interactive environment

```python
>>>import pdb
>>> pdb.pm() # post mortem
can use print statements to find surrounding context

(pdb) list # to see surrounding code
(pdb) quit

```

2. Use import pdb; pdb.set_trace() in python file as debug point to launch debugger
python3 filename

### Lesson 2 : Python Structure and Execution Models. 

Add mortage.py 

> variable declaration 
> indentation consistency  ( Controversial) - generally 4 space charcater   - No tab  


formatted printing (watch 2.2 )
name 
print(










