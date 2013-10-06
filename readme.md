foo_winamp_spam 0.99
=======================

Improves upon Selyb's version 0.98 (http://home.comcast.net/~selyb/ which was, fortunately, not broken!) which, in turn, was built upon Chronial's 0.96 (https://github.com/Chronial/foo_winamp_spam), which was based upon R1CH's original version.

What's new
----------
Version 0.99
* Fixes unicode support, properly converting to UTF16 before setting the title
* Fixes the "Calls metadb_handle->get_info_locked(info), does not check the return value, accesses random garbage because info stays uninitialized." bug

Version 0.98

* Play/Pause now toggles play/pause instead of only pausing (code was already there but commented out by a previous dev)

Version v0.97

* fixed IPC_IPLAYING, now returns 3 if paused
* swapped Rewind and Start of playlist to correct message numbers
* mapped WM_COMMAND 40061 to Rewind
* swapped FF and End of playlist to correct message numbers
* mapped WM_COMMAND 40060 to FF

Download
--------

Installation
------------
Foobar 1.1 and newer should be able to install the component without issues. 
If that does not work, extract the dll from the package (the .fb2k-component file is a .zip file) and place it in the correct components folder for your foobar version.
For older versions, you will need to compile the plugin using an older SDK (or preferable, update your foobar2000 installation).

Compilation
-----------
This project was built using the Foobar SDK 2011-03-11.
The SDK is expected in ../foobar2000 and ../pfc

Known Bugs
----------
* None, but I've only modified a few parts of the plugin. There may be bugs, and I would appreciate any reports of such.

Testing
-------
* Tested with foobar2000 v1.2.9 on Windows 8 Pro x64