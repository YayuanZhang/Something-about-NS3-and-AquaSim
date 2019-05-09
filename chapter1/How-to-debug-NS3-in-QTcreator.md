# step 1 dynamic loader
`sudo gedit /etc/ld.so.conf`

add the `<path>/build` to the end of the file
  
`sudo ldconfig`

ldconfig creates the necessary links and cache to the most recent shared libraries found in the directories specified on the command line, in the file /etc/ld.so.conf, and in the trusted directories,/lib and /usr/lib

# step 2 debug  a "waf" built ns-3 application
In qtcreator, first set click Projects on the left and then under Targets and Desktop select Run. 

Under Run Configuration, set Executable to `<path>/build/XXX/ns3-cppname-debug`

Use Debug->Start Debugging->Start Debugging.

