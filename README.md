# barnard

barnard is a terminal-based client for the [Mumble](https://mumble.info) voice
chat software.

![Screenshot](https://i.imgur.com/B8ldT5k.png)

## Installation

Requirements:

1. [Go](https://golang.org/) - sudo apt-get install goland
2. [Git](https://git-scm.com/) - sudo apt-get install git
3. [Opus](https://opus-codec.org/) development headers - sudo apt-get install libopus-dev
4. [OpenAL](http://kcat.strangesoft.net/openal.html) development headers - sudo apt-get install libopenal-dev

To fetch and build:

    export GOPATH=$HOME/go 
    go get -u github.com/savvamadar/barnard

After running the command above, `barnard` will be compiled as `$(go env GOPATH)/bin/barnard`.

## Manual

### Usage

To run: $GOPATH/bin/barnard [-flags]

### Flags

- flag: default
- server: localhost:64738
- username:
- password:
- insecure:
- certificate:
- voiceon:

Sample: $GOPATH/bin/barnard -server 127.0.0.1:64738 -username myUser -insecure -voiceon

This will connect myUser to the 127.0.0.1 mumble ip running on port 64738 and won't check for certificates and will have the voice on by default.

### Chat Commands (useful for SSH)

- quit: disconnects
- exit: disconnects
- voice: toggles voice on or off

### Key bindings

- <kbd>F1</kbd>: toggle voice transmission
- <kbd>Ctrl+L</kbd>: clear chat log
- <kbd>Tab</kbd>: toggle focus between chat and user tree
- <kbd>Page Up</kbd>: scroll chat up
- <kbd>Page Down</kbd>: scroll chat down
- <kbd>Home</kbd>: scroll chat to the top
- <kbd>End</kbd>: scroll chat to the bottom
- <kbd>F10</kbd>: quit

## License

GPLv2

## Fork Author

Savva Madar (<savva.madar@gmail.com>)

## Original Author

Tim Cooper (<tim.cooper@layeh.com>)
