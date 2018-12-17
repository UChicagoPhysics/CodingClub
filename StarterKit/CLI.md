# Command Line Interface Tutorial

The command line interface (CLI) is a tool that is both extremely powerful and extremely abstruse.
A holdover from early computing, the CLI used to be the only way one could interact with the computer; as such, its commands are often archaic and composed of only two or three characters (to minimize how much you need to type), and it does not explain itself unless you know how to ask.
However, it is still widely used, and learning how to do so opens up many possibilities in computing.

## How to get here

Depending on your operating system (OS), there are a few different ways to get to the CLI.
Most CLIs are terminal emulators, which means that they are graphical user interface (GUI) applications that run a terminal inside of a window (i.e. like a normal application).
Furthermore, most terminal emulators use the `BASH` shell, which just means that they use the `BASH` scripting language for their commands; effectively, you get the same commands and the same behavior with any terminal that uses `BASH`.

### macOS

Apple provides a full-featured CLI through `Terminal.app`, found in the `~/Applications/Utilities/` folder.
You can also open up `Spotlight` with <kbd>&#8984;</kbd> + <kbd>SPACE</kbd> and simply start typing `Terminal`.
No additional setup is necessary at this point.

### Windows

Microsoft's prebundled CLI, `Cmd.exe`, lacks some important features that we will want for programming (e.g. `git`), so we recommend installing another terminal emulator.
We have found that doing a full download of [Cmder](http://cmder.net/) works well; there is also Microsoft's [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/about) for those more familiar with Linux.

### Linux

As with macOS, most (if not all) Linux distributions come prepackaged with fully usable terminal emulators and should be usable out of the box.
The location of the terminal will depend on the distribution, but most should be fairly easy to find.

### Chrome OS

Google's Chromebook operating system now (for versions 53 or newer) [supports Android apps](https://support.google.com/googleplay/answer/7021273?hl=en).
In particular, [Termux](https://termux.com/) gives you access to a fantastic termunal emulator similar to what you would find in a more traditional Unix (Linux, macOS, etc...) desktop environment.
We recommend updating packages and allowing `Termux` to talk to the rest of the system:
```
pkg update
pkg upgrade
termux-setup-storage
```
If you come across a command that you don't have, you should be able to install it with `pkg`; for instance, `pkg install git`.

## How to navigate

There are three basic commands that helps us get around in the terminal: `pwd`, `ls`, and `cd`.
- `pwd` (print working directory) tells you where you currently are.
- `ls` (list) shows you whats inside the current working directory.
- `cd` (change directory) following by a directory name lets you move to that directory.

Let's try these out (the following is copied and pasted from my Terminal):
```
$ pwd
/Users/sidneymau
$ ls
Applications/ Library/      Public/       rust_scratch/ ugali.sh
Desktop/      Movies/       bin/          sid           update.sh
Documents/    Music/        git/          smau.sh       vhdl_scratch/
Downloads/    Pictures/     miniconda3/   software/
$ cd Documents/
$ pwd
/Users/sidneymau/Documents
$ ls
ATLAS/               Zoom/                random/
DES/                 apartment/           resume/
GitLab/              cs152/               taxes/
TASIS/               cs161/               uchicago/
Wolfram Mathematica/ music/               zac_photos/
$
```
Some navigational shorthands to use with `cd` are
- `.` (current directory)
- `..` (previous directory)
- `~` (home directory)
