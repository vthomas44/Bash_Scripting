# finder.sh
This script recursively searches for a given string in all files within a specified directory.
- filesdir – the path to the directory
- searchstr – the string to search

# writer.sh
This script creates a file with a given path and writes a specified string to it.
- writefile – the full file path (including file name)
- writestr – the content to write into the file

# aesdsocket-start-stop
This init script manages the `aesdsocket` daemon, allowing it to start, stop, or restart during system boot and shutdown.
- start – launches the daemon in the background with `-d` flag
- stop – gracefully stops the daemon and removes its PID file
- restart – stops and then restarts the daemon.

Full working code available at [assignments-3-and-later-vthomas44/server/](https://github.com/cu-ecen-aeld/assignments-3-and-later-vthomas44/tree/main/server)

# S98lddmodules
This init script manages loading and unloading of Linux Device Driver (LDD) modules (`scull`, `faulty`, `hello`) and creates/removes their corresponding device nodes.
- start – loads modules with `modprobe` and creates `/dev` nodes using major numbers from `/proc/devices`
- stop –  removes device nodes and unloads the modules using `rmmod`

Full working code available at [assignment-5-vthomas44\base_external/rootfs_overlay/etc/init.d/S98lddmodules](https://github.com/cu-ecen-aeld/assignment-5-vthomas44/blob/main/base_external/rootfs_overlay/etc/init.d/S98lddmodules)
