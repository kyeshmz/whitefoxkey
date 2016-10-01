# My Whitefox Keyboard Configuration for macOS

This is my configuration for [Matt3o's Whitefox keyboard](https://input.club/whitefox) (The True Fox layout).

![Whitefox, config ](https://raw.githubusercontent.com/kkshmz/whitefox-config/assets/keyboard-diagram.png)

Download it and flash by using `dfu-util -D kiibohd.dfu.bin` with terminal.
I will link the tutorial here, once I am finished with it, because I know the one that Massdrop has is super lacking.

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

 ![Whitefox, config ](https://raw.githubusercontent.com/kkshmz/whitefox-config/assets/keyboard-modifier.png)
