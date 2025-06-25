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
