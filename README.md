# Zoom Meeting Shortcut Tool

This repository contains a command-line tool that opens the Zoom app with the provided link. The tool includes an Apple Script that is compiled into a standalone app. You can easily drag the app to the macOS dock or any preferred location for quick access.

## Usage

To create an executable macOS app that opens a Zoom room directly, use the following command:

```
Usage: create_app.sh [-p|--png-path <arg>] [-h|--help] <zoom-link>
        <zoom-link>: Link of the zoom room you want to join e.g: "https://us02web.zoom.us/j/<MEETINGID>?pwd=<PWD>" 
        -p, --png-path: path to png file that will be used as an icon (default: 'icon.png')
        -h, --help: Prints help
```
## Requirements

Make sure you have `imagemagick` installed before running this tool. You can install it using Homebrew:

```shell
brew install imagemagick
```

## Resources Used

- The supplied icon was created by [Alexandr Martinov](https://www.iconfinder.com/icons/7150137/coffee_maker_cup_cafe_mashine_icon)
- Command-line argument handling created by [argbash](https://argbash.dev/)
- Several Stack Overflow posts and Gists were referenced:
  - [How to create a temporary file in a shell script](https://unix.stackexchange.com/questions/181937/how-create-a-temporary-file-in-shell-script#comment302878_181939)
  - [AppleScript to open URL](https://gist.github.com/jamieweavis/b4c394607641e1280d447deed5fc85fc)
  - [Invalid command code 'f' in sed](https://stackoverflow.com/questions/29081799/sed-1-invalid-command-code-f)