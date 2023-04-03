<!-- Header -->
![](images/keybs.jpeg)

<!-- Body -->
# Keymaps

This repository contains the keymaps for my split keyboards, with an explanation and diagrams of each layer's functionality.

The repository currently contains my keymaps for:

- [Duckyb](https://github.com/duckyb)'s Urchin Keyboard
    - Runs ZMK firmware built through Github Actions
    - Uses nice!nano wireless controllers and nice!view displays
    - See `keymaps/urchin`
- [SplitKB](https://www.google.com/search?client=safari&rls=en&q=corne+aurora&ie=UTF-8&oe=UTF-8)'s Aurora Corne
    - Runs QMK firmware built locally
    - Uses the Elite-Pi controller (RP2040 based)
    - Utilizes 34 keys (out of the 42 available)
        - ***34 keys is all you need***
    - See `keymaps/aurora-corne`


## Layers
All keyboards share the same core hardwired layers (built into the controller's firmware) and software functionality layers (based on external applications).


### Core layers
There are 4 core layers. These layers, built into the keyboard's firmware, are used for everyday typing and coding. They are all accessed through the main layer. Each has its own purpose, with the *Alpha* layer containing all letters, the *NumNav* layer having the numbers and navigation keys and the *Symbol* layer having everything else. In order:

- `Alpha layer`
    - Default layer
    - Contains all letters in a **QUERTY** arrangement
    - Uses mirrored **home row mods** for `⌘ ⌥ ^`
    - Implements Hyper `♡` and Meh `☆` keys with tap and hold
    - It is used to access al other layers
        - Uses the right cluster to access the `NumNav` and `Symbol` layers
        - Uses the `N` and `B` keys to access the one-handed layer

- `NumNav layer`
    - Contains the number row in a laptop-style arrangement
    - Has the navigation keys with hard-coded modifiers, for easier navigation in macOS
    - Includes one-handed media controls and two-handed volume controls
    - Includes ` ⏎  ⎋  ⇥` and ` ⌫ ` keys, designed to be easily chorded

- `Symbol layer`
    - Includes all main symbols
    - Keys are arranged with positional semantics in mind
    - The most used keys are concentrated around the home row

- `One-handed layer`
    - The layer is mirrored in both the left and right halves of the keyboard
    - It is accessed from the main layer with a index (or thumb) finger press on `N` or `B`
    - Includes easy access to media controls and arrow navigation

### Functionality layers
There are 3 additional software functionality layers. These layers are not hardwired into the software, rather they use third-party applications to quickly launch programs, manage windows and spaces.

- `App launcher layer`
    - Uses the `Meh☆` key to quickly launch (or bring into focus) the most frequently used apps
    - The `Meh☆` key is accessed via a holding the space key
    - App launching is implemented using the [Thor launcher](https://apps.apple.com/us/app/thor-launcher/id1120999687?mt=12)

- `Window management layer`
    - Includes multiple shortcuts for manipulating the focused window
    - Shortcuts are mapped to a combined press of `⌥` and `^` (`jk` on the right half), which allows all shortcuts to be swiftly chorded
    - Shortcuts are implemented using [Rectangle](https://rectangleapp.com)

- `Space management layer`
    - This layer is accessed by pressing `^` and `⇧`
    - Enables **pure** keyboard based movement across macOS
    - Quickly switches between `spaces`, `windows` and `focus` across multiple app instances
    - Shortcuts are implemented using native macOS and [Amethyst](https://github.com/ianyh/Amethyst)


It is worth noting that in order to be fully keyboard-based you cannot use macOS's fullscreen (accessed through the green button in the top-left corner of a window). Instead, you can fullscreen the active window with a window management shortcut (`⌥ ^ + S` for me). While you lose some screen real state, you can be more agile while switching windows and you keep the menu bar always visible.

Ideally, you should create a discrete number of [spaces](https://support.apple.com/guide/mac-help/work-in-multiple-spaces-mh14112/mac) and distribute your windows across them. You can then use the space management layer to quickly hop between them, keeping everything organized and, more importantly, ***ergonomic***.

## Diagrams

Here are diagrams for all layers. The Affinity Designer template used to create these diagrams is stored in `diagrams/template`.

**Color legend**:
- `Orange`: Home row modifiers
- `Green`: Tap and hold actions
- `Blue`: Hold-to-layer action


### Main layer


`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/Layer1_L.png) |  ![](/images/Layer1_R.png)

### NumNav layer
`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/Layer2_R.png)  |  ![](/images/Layer2_L.png)


### Symbol layer

`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/Layer3_R.png)  |  ![](/images/Layer3_L.png)


### One-handed layer

`Right (mirrored)`       |
:-------------------------:|
![](/images/Layer5_R.png)  |


## Functionality Layers

### App Launcher Layer

`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/AppLayerLeft.png)  |  ![](/images/AppLayerRight.png)


### Window Management Layer

`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/WindowManagementKeymapLeft.png)  |  ![](/images/WindowManagementKeymapRight.png)



### Space Management Layer
`Left`       |  `Right`
:-------------------------:|:-------------------------:
![](/images/SpaceSwapKeymapLeft.png)  |  ![](/images/SpaceSwapKeymapRight.png)

