symbolicatecrash Path :

/Applications/Xcode6.4.app/Contents/SharedFrameworks/DTDeviceKitBase.framework/Versions/A/Resources/symbolicatecrash

/Applications/Xcode8.2.1.app/Contents/SharedFrameworks/DVTFoundation.framework/Versions/A/Resources/symbolicatecrash

Run : 
export DEVELOPER_DIR='/Applications/Xcode6.4.app/Contents/Developer'

export DEVELOPER_DIR='/Applications/Xcode8.2.1.app/Contents/Developer'

export DEVELOPER_DIR='/Applications/Xcode9GM.app/Contents/Developer'

symbolicatecrash /path/to/MyApp_2012-10-01_Device.crash /path/to/MyApp.app.dSYM.



//xcode9GM
atos -o ETNet.app.dSYM/Contents/Resources/DWARF/ETNet -l 0x102b40000 0x0000000102b8ccec

//Self make symbolicatecrash shell script
sh re-sym [crash log] [dSYM] [outfile]
e.g sh re-sym ./ETNet-20180712.ips ETNet.app.dSYM re-symbol_.txt
