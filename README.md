# gadgets-hpcalc

HPCalc for the gadgets of [polpo](https://github.com/polpo-system/polpo): a calculator in reverse
Polish notation, as the HP calculators, with integer, real and bit functions.

```
portia.Install gadgets-hpcalc
```

## Using

    Desktops.OpenDoc HPCalc.Panel     the calculator
    HPCalc.Open                       makes the panel anew (store it with Desktops.StoreDoc)

## What is here

    src/Conversions.Mod     conversions between number formats, which HPCalc uses
    src/HPCalc.Mod          the calculator
    share/HPCalc.Panel      its panel
    tools/HPCalc.Tool
    test/HPCalcTest.Mod

HPCalc is by Patrik Reali. The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    HPCalcTest.Run      3 checks: the calculator model and gadget made, the panel opened; it
                        needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
