# easy65C02
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Easy65C02 is an fork of Easy6502 by Nick Morgan which support additionnals opcodes found in the WDC 65C02 CPU.

See http://eddybeaupre.github.io/easy65C02/ for the live site.

The original 6502 version can be found at https://skilldrick.github.io/easy6502/

This simulator load it's code a $E000 instead of $0600. Mostly to simulate running from ROM instead of RAM.

## Supported new opcodes

|instruction|OpCode|Implemented|Description|
|-----------|------|-----------|-----------|
|BRA r|0x80|Yes|Branch Always|
|STZ d|0x64|Yes|Store Zero (Zero Page)|
|STZ d,X|0x74|Yes|Store Zero (Zero Page, X)|
|STZ a|0x9C|Yes|Store Zero (Absolute)|
|STZ a,X|0x9E|Yes|Store Zero (Absolute, X)|
|ORA (d)|0x12|Yes|OR with Accumulator (Indirect)|
|AND (d)|0x32|Yes|AND with Accumulator (Indirect)|
|EOR (d)|0x52|Yes|EOR with Accumulator (Indirect)|
|ADC (d)|0x72|Yes|Add to Accumulator with Carry (Indirect)|
|STA (d)|0x92|Yes|Store Accumulator (Indirect)|
|LDA (d)|0xB2|Yes|Load Accumulator (Indirect)|
|CMP (d)|0xD2|Yes|Compare with Accumulator (Indirect)|
|SBC (d)|0xF2|Yes|Subtract from Accumulator with Borrow (Indirect)|
|BIT d,X|0x34|Yes|Bit Test with Accumulator (Zero Page, X)|
|BIT #|0x89|Yes|Bit Test with Accumulator (Immediate)|
|BIT a,X|0x3C|Yes|Bit Test with Accumulator (Absolute, X)|
|INC|0x1A|Yes|Increment Accumulator by one (Implied)|
|DEC|0x3A|Yes|Decrement Accumulator by one (Implied)|
|PHY|0x5A|Yes|Push Y to Stack|
|PLY|0x7A|Yes|Pull Y from Stack|
|PHX|0xDA|Yes|Push X to Stack|
|PLX|0xFA|Yes|Pull X from Stack|
|TSB d|0x04|No|Test and Set Bits (Zero Page)|
|TSB a|0x0C|No|Test and Set Bits (Absolute)|
|TRB d|0x14|No|Test and Reset Bits (Zero Page)|
|TRB a|0x1C|No|Test and Reset Bits (Absolute)|
|JMP (a,X)|0x7C|Yes|Jump (Absolute, X)|

Full list of 65C02 OpCodes: https://feertech.com/legion/reference65c02.html

Official WDC datasheet for the 65C02: https://www.westerndesigncenter.com/wdc/documentation/w65c02s.pdf
