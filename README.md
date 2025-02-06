# OIO
Upython code to copy a file between 2 boards by uart commands.
The ask file is on the board which act; the responses file is on the board which react. On the react board the script have to run.
For moment works just with upython... The board's parameters are done with a Pybnano_V2. I will add a pure python form.
On the board which act, you can write :
"

import ask

ask.copy('myfile') ## it will copy the file on the other board on this board with the same name.

ask.copy2('myfile') ## it will copy the file from this board on the other board with the same name.

"
