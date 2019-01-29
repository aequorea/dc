### dc
design compiler -- generate a netlist from a text description of an electronic design

Compile with fpc (free pascal compiler). I think it's really nice that software from 1990 compiled without changes and "just worked." The compiler didn't even complain about the vestigial control-z that DOS put at the end of the file.

Takes a .dc file as input. When you run the program do not include the file extension, just the filename without the extension. The output is a .net file which has the netlist.

This software exists because back in the day, schematic capture and PC layout were not always so well integrated. I'd draw the schematic by hand or with something like Mac Draw and then make a .dc file. The .net file was a netlist file that I could compare to a netlist generated by the pc layout software which was Tango PCB back then. This way I could verify the pc board at least matched the text description of the schematic if not the schematic.

dc.pas -- the source code
module.dc -- sample design description for the Palomino battery charger
module.net -- output from the design compiler
