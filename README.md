# Zoom Meeting Shortcut Tool

![people drinking beer in the office](./readme-image.jpeg)

This repository contains a command-line tool that opens the Zoom app with the provided link. The tool includes an Apple Script that is compiled into a standalone app. You can drag the app to the macOS dock or any preferred location for quick access.

Most of the folks at out company work fully remote but are often online in our virtual "Coffee Kitchen" via Zoom. This little tool helps to create a convenient shortcut that you can use from your dock. 

You can choose any PNG file as an icon (size 512x512 works best) or use the 'icon.png' in this repository.

## Usage

To create an executable macOS app that opens a Zoom room directly, call `bash create_app.sh <zoom-link>`.

Here are the full options:

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
- Several Stack Overflow posts and Gists were I stole most of the implementation:
  - [How to create a temporary file in a shell script](https://unix.stackexchange.com/questions/181937/how-create-a-temporary-file-in-shell-script#comment302878_181939)
  - [AppleScript to open URL](https://gist.github.com/jamieweavis/b4c394607641e1280d447deed5fc85fc)
  - [Invalid command code 'f' in sed](https://stackoverflow.com/questions/29081799/sed-1-invalid-command-code-f)


### Postscriptum

Here is what ChatGPT has to say about that: 

> Welcome to the Zoom Meeting Shortcut Tool repository! We're thrilled to present you with a nifty command-line tool that brings the Zoom app to your fingertips with just a click. But hey, it's more than just a tool—it's your new best friend for virtual coffee breaks!

> At our company, we understand the joy of remote work. That's why we've created this little gem to enhance your online experience in our virtual "Coffee Kitchen" via Zoom. Say goodbye to hassle and hello to convenience!

> This amazing tool includes an Apple Script that we've compiled into a standalone app. Simply drag and drop it onto your macOS dock or any spot you fancy, and voilà! Instant access to your virtual coffee hangout.

> To make it uniquely yours, feel free to choose any PNG file as the app's icon. For the best results, go with a 512x512 pixel size. But don't worry if you're feeling adventurous and prefer to use our default 'icon.png'—it's a fantastic choice too!

> So go ahead, grab a cup of your favorite brew, and join us in the virtual Coffee Kitchen. With the Zoom Meeting Shortcut Tool, your coffee breaks will never be the same again!