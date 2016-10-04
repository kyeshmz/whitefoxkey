# My Whitefox Keyboard Configuration for macOS

This is my configuration for [Matt3o's Whitefox keyboard](https://input.club/whitefox) (The True Fox layout).

![Whitefox keyboard, full](https://raw.githubusercontent.com/kkshmz/whitefoxkey/master/docs/keyboard-diagram.png)

## What is the Whitefox keyboard?
The Whitefox keyboard is a 65% keyboard, with the PCB designed by the [Input Club](http://input.club/), who also designed the Infinity keyboard.
The keycaps are PBT Cherry keycaps, which are designed by Matt3o, the legendary keyboard master himself.

The firmware that is used with this project is [KLL](https://input.club/kll) made by HaaTa, a member of the Input Club.

The KLL is a dynamic and functional language designed to work with all types of input devices and was created after HaaTa was fed up with defining Colemak for every single keyboard.


It is avaliable through [Massdrop](https://www.massdrop.com/buy/the-whitefox-keyboard) , which can be bough assembled or in parts.
More can be understood on their [github](https://github.com/kiibohd/controller) and the [firmware pdf](https://www.overleaf.com/read/zzqbdwqjfwwf).

Install that thing from the Apple store called [Xcode](https://developer.apple.com/xcode/).
`xcode-select --install`
`sudo xcodebuild -license`

I recommend not using Macports to add any of the extensions that is needed for most of the installation. The project is basically dead.

Rather, use [homebrew](http://brew.sh/index.html).


It can be installed using 

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"` 

, but you already knew that.

Install the extensions,
`brew install dfu-util`



Enter the DFU Flash Mode for the keyboard by clicking on the hole inside of the back with a paperclip or something.

![Whitefox, Keyboard Flash](https://raw.githubusercontent.com/kkshmz/whitefoxkey/master/docs/keyboard-flash.jpg)

Flash by directing to the directory you installed to
```
cd Downloads
cd < directory with kiibohd.dfu.bin >
```
and then use `dfu-util -D <kiibohd.dfu.bin>`

Finally, go over to the modifier keys in the macOS settings.


![Whitefox, Apple Settings](https://raw.githubusercontent.com/kkshmz/whitefoxkey/master/docs/modifier-settings.png)

![Whitefox keyboard, full](https://raw.githubusercontent.com/kkshmz/whitefoxkey/master/docs/modify-keys.png)

![Whitefox keyboard, Apple Modifier](https://raw.githubusercontent.com/kkshmz/whitefoxkey/master/docs/keyboard-modifier.png)


## Some basic tips on the configurator
* ƒ[num]  Activates layer while the key is held (like shift)

* LOCK-[num]
Activates layer until the key is pressed again (like caps lock)

* LATCH-[num]
Activates the layer for a single keypress (like a dead key for international character input)

* NONE
By default, layers stack so that keys on the layer below remain accessible unless they are overridden. Use NONE if you want a layer to override a lower layer with a non-action.

* Stacking layers
The Main layer is always active at the bottom. Above that, layers are stacked in the order they are activated, not by their number. If layer 3 is LOCKed and then layer 2 is ƒ shifted, any keys defined by layer 2 will override keys on layers 3 and Main. The layer order is displayed on the LCD.
It’s possible to stack up to 5 layers at once in any combination of the 3 methods (lock, latch, ƒ-shift), which is as insanely powerful as it is confusing.

## Some of the features that are with this guide
* Modifier keys are setup according to Window & Apple standard
 - CTRL = CTRL
 - ALT = ALT/OPTION
 - CMD = GUI
* Included the function keys where they are allocated on macOS keyboards, which will probably change with the new laptop. Who knows.

