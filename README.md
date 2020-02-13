# WSL Dev Setup

This guid records my personal setup for WSL on a Windows10 computer. It is a reminder for myself, however it may be useful for some friends aiming to quickly set up developer environment on WSL.

- [WSL Dev Setup](#wsl-dev-setup)
  - [WSL](#wsl)
  - [Visual Studio Code](#visual-studio-code)
  - [Git](#git)

## WSL

Follow the [offical installation guide](https://docs.microsoft.com/en-us/windows/wsl/install-win10).

Run `wsl` from a command prompt to enter subsystem for Linux.

[WSL2](https://docs.microsoft.com/en-us/windows/wsl/wsl2-index) is a new version of increasing file system performance.

## Visual Studio Code

Follow the [offical installation guide](https://code.visualstudio.com/docs/remote/wsl#_installation).

*Tip:* WSL1 has some [known limitations](https://code.visualstudio.com/docs/remote/wsl#_known-limitations). Offical guidelines give some advices, but I've found that simply exiting VSCode is very effective for problems caused by the file watcher : )

## Git

Most Linux distributions has a pre-installed version of [Git](http://git-scm.com/), but we can intall our own through apt-get to allow easy upgrades and not interfere with the system version. To do so, simply run: `apt install git`.

[https://gitignore.io/](https://gitignore.io/) is useful to create .gitignore files.

[Customize git](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration). Make sure `core.editor` is set to your favourite text editor : )

[gitk](https://git-scm.com/docs/gitk) is a Git GUI. We can install it easily:

1. Run `apt install gitk`.

2. Download the [Xming X Server for Windows](https://sourceforge.net/projects/xming/).

3. Install Xming. The default settings should work just fine.

4. Run Xming.

5. Run `gitk`.
