Python debugging

1. python3 -i filename [input_parameters]
Runs the program and drops you at interactive prompt after the error. Values can be checked in interactive environment

>>>import pdb
>>> pdb.pm() # post mortem
can use print statements to find surrounding context

(pdb) list # to see surrounding code
(pdb) quit

2. Use import pdb; pdb.set_trace() in python file as debug point to launch debugger
python3 filename


