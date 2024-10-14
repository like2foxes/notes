In order to yank all lines withing range that match a pattern I can use:
:[range]g/{pattern}/y {register}

The register must be a capital letter which means vim will append to the register. Otherwise it will override the former line and in the end only the last line matching the pattern will be yanked.

i.e:
:1,5g/koko/y A
Append all lines from line 1 to line 5 that contains the pattern "koko" and append them to the a register.
