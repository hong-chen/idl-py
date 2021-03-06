# idl-py

## Dependencies

- Python 3.6
  - os
  - sys
  - [pexpect](https://pexpect.readthedocs.io/en/stable)

    To install `pexpect`, try `pip install pexpect` in a terminal.

- [IDL](http://www.harrisgeospatial.com/ProductsandTechnology/Software/IDL.aspx)
  - To get IDL running in a terminal, add `export PATH="/Applications/exelis/idl85/bin:$PATH"` to `.bashrc` (or `.bash_profile`).
---

## Description

Automatically complile the `.pro` file and provide a sample
line to run the procedures or functions in the targeted file.

---

## How to use

For a target file, e.g. `test.pro`, run the following command in a terminal

```bash
idl-py test.pro
```
---

## Example

After run
```bash
idl-py muslope.pro
```

The output on the screen will look like
```text
IDL Version 8.5.1, Mac OS X (darwin x86_64 m64).
(c) 2015, Exelis Visual Information Solutions, Inc., a subsidiary of Harris Corporation.
Installation number: 100-3091.
Licensed for use by: University of Colorado - Boulder (MAIN)

IDL> .r sub_muslope.pro
% Compiled module: MUSLOPE.

+ How to run
MUSLOPE, sunzen, sunaz, nrmzen, nrmaz
-

Hit "Enter" to continue...

```
---

## Note

Add the following in to `.bashrc`

```
alias idl="idl-py"
```
