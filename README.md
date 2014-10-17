shell-recorder
==============

A shell commands recorder

# Installation

1. Clone the repository: `git clone git@github.com:viniciusffj/shell-recorder.git`
2. Make files executable: `chmod +x start-record stop-record`
3. Put files available on path, for example `sudo cp start-record stop-record /usr/local/bin/`

# Usage

shell recorder is simple to use:

* Start recording with: `. start-record`
* Type your commands
* End recording with: `. stop-record`

For example:

```
$ . start-record
$ ls
$ git status
$ git diff .
$ . stop-record script
```

If we look at script: 
```
ls 
git status
git diff .
```

If we do not pass parameter to `stop-record` the commands will be save at `~/.sr/result-recording`
