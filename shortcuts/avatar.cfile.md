__
^@(.+)$
__
return "![["+$1+".png#avatar]]\n\n>[!dialouge]\n>**"+$1+"//** ";
__
This will trigger in ironsworn.css to create an avatar based on the input with proceeding text in a callout box.