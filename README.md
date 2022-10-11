# Exagear-ARMv7-ARMv8-Cracked
Dynamic binary translator Revision 3003. With activated Licence!

ubt_x32a32_alv7 -> armv7
ubt_x32a32_alv8 -> armv8

./ubt_x32a32_alv7 --help
Usage: ./ubt_x32a32_alv7 [compiler_options] -- <guest_executable> [guest_executable_options]

General options
--help/-h - Shows help screen
--version/-v - Product version

Virtual File System (VFS) options
--path-prefix <param> - Path to the guest FS image
--opaths-list <param> - Path to the list of overriden FS elements
--vpaths-list <param> - Path to the list of substituted FS elements
--vfs-kind <param> - Selection of the primary and secondary fs roots (valid values are 'host-first' and 'guest-first')
--fs-root <param> - Path to root of the guest file system (chroot emulation)
--fs-root-shmfd <param> - File descriptor number used for inteprocess filesystem root info storage
--hifd-base <param> - Highest file descriptor of HiFd area
--tmp-dir <param> - Path to the directory to keep temporary files in

#!/bin/sh
exec /usr/bin/ubt_x32a32_alv7 --path-prefix /opt/buster --vpaths-list /usr/sbin/vpaths-list -- $@

#!/bin/sh
exec /usr/bin/ubt_x32a32_alv7 --path-prefix /opt/buster --vpaths-list /usr/sbin/vpaths-list -- /usr/bin/wine $@ 

