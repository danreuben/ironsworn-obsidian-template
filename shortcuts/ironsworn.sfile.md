__
^@(.+)*$
__
return "![["+$1+".png#avatar]]**"+$1+"//**";
__
@+input - Expands into "![[input.png#avatar]]**input//**".  This will trigger in ironsworn.css to create a avatar based on the input with proceeding text in a callout box.
__