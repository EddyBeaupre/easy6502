# easy65C02
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Easy65C02 is an fork of Easy6502 by Nick Morgan which support additionnals opcodes found in the WDC 65C02 CPU.

See http://eddybeaupre.github.io/easy65C02/ for the live site.

The original 6502 version can be found at https://skilldrick.github.io/easy6502/

## Supported new opcodes

|instruction|OpCode|Implemented|Description|
|-----------|------|-----------|-----------|
|BRA r|0x7A|No|Branch Always|
|STZ a|0x9C|No|Store Zero (Absolute)|
|STZ a,X|0x9E|No|Store Zero (Absolute, X)|
|ORA (d)|0x12|No|OR with Accumulator (Indirect)|
|AND (d)|0x32|No|AND with Accumulator (Indirect)|
|EOR (d)|0x52|No|EOR with Accumulator (Indirect)|
|ADC (d)|0x72|No|
|STA (d)|0x92|No|
|LDA (d)|0xB2|No|
|CMP (d)|0xB2|No|
|SBC (d)|0xF2|No|
|TSB d|0x04|No|
|TRB d|0x14|No|
|BIT d,X|0x34|No|
|STZ d|0x64|No|
|STZ d,X|0x74|No|
|BIT #|0x89|No|
|INC A|0x1A|No|
|DEC A|0x3A|No|
|PHY|0x5A|Yes|
|PLY|0x7A|Yes|
|PHX|0xDA|Yes|
|PLX|0xFA|Yes|
|TSB a|0x0C|No|
|TRB a|0x1C|No|
|TRB a|0x1C|No|
|BIT a,X|0x3C|No|
|JMP (a,X)|0x7C|No|
|STZ a|0x9C|No|
|Stz a,X|0x9E|No|
