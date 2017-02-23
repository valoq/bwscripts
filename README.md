bwscripts
========
Bubblewrap example scripts

This repository contains some tools for working with bubblewrap as well as example profile scripts for several programs to show how bubblewrap can be used to sandbox applications.



Install
-------

To automatically use the sandboxed applications profiles, copy the scripts to /usr/local/bin and make them executable. By default a seccomp bpf file is expected in that directory as well. Use the exportFilter program to generate the seccomp bpf file. You can create individual filters by specifying syscalls to be blacklisted or whitelisted using the defined macros.



Disclaimer
----------

This repository is not associated with the official bubblewrap project




Warning
-------

Using the provided scripts to sandbox linux desktop applications only provides limited protection as there are several weak points like the X-Window-Server and Dbus IPC that need to be isolated as well to prevent sandbox escape. 