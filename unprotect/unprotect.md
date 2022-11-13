If "new" device fail to program :
- in xsvfduino "TDO mismatch"
- in xc3sprog "Erase still running 00"
...it might be write protected.

Do the following :
1/ open ISE iMPACT
2/ "Create XSVF file" for the target chip
3/ "Set Erase Properties"
4/ check "Override Write Protect"
5/ "Erase"
6/ "Stop Writing to XSVF File"
7/ program the xsvf file with xsvfduino
