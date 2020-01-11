#### This is a project to porting TELNET client from FreeBSD release 11.3.
#### to a MasOS (Darwin).

If you are using QEMU, SimH or any other emulator you need to connect to a console in the emulator.
To connect to a console is using TELNET localhost PORT_NUMBER command,
but MacOS (Darwin) does not has a telnet client.

##### How to compile on a MacOS (Darwin)
Simply launch make utility on a terminal window:
```
$ make
```

p.s.
TELNET has been tested on a:
Darwin 17.7.0 Darwin Kernel Version 17.7.0
Sun Dec  1 19:19:56 PST 2019; root:xnu-4570.71.63~1/RELEASE_X86_64 x86_64
