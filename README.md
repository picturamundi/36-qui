# Pictura Keyboard Layout Manual

Pictura is an ergonomic keyboard layout compatible with devices running the ZMK keyboard firmware.

For all information on how ZMK works, how to use this layout, how to edit it, and so on, see the official [ZMK documentation]((https://zmk.dev/docs)).


## At a glance…

**For users who want to skip the explanation of this layout's design and jump right in, here are are a few quick should-knows:**

- Made with a [Microdox](https://boardsource.xyz/store/5f2e7e4a2902de7151494f92) in mind, which has a very retracted thumb-cluster. Outer and middle thumb keys could probably be swapped for something like a Corne.
- For commands with no dedicated ZMK key-code (e.g. navigate backward and forward on webpages), I'm using shortcuts key-combos that work on my personal machine, but they may have to be customized for other devices. See the layout legend below for what these shortcuts are supposed to actually do.

How does this layout compare to the popular 36-key [Miryoku layout](https://github.com/manna-harbour/miryoku/tree/master/docs/reference)? With the understanding that this is a much less fully-featured project which was designed with only my own personal use in mind, here are nonetheless the key advantages for me: 
  - Tap-Shift for less finger strain when typing, although there's also the option of a tradition hold-shift in the form of a home-row mod
  - Tab-control on home-layer… in fact in general [there's just more that's accessible on the home layer](#1-home-accessible-keys)
  - One-handed layers for mouse-friendly use
  - DVORAK alphas but optional [QWERTY command shortcuts](#qwerty-commands-and-hand-matching)


## Ergonomic considerations

This isn't the place to belabor points about ergonomic layouts, or sub-40% keyboards, or the advantages of using a custom firmware, all of which aren't unique to this layout and have been written about elsewhere. I'll summarize these general features in this brief list:

- Hardware 
  - **36-key layout**: Minimise wrist movement for touch-typists by placing all keys within immediate reach of fingers resting on the home row. Also makes it easier to type without ever looking at the keyboard, ever for numbers, function keys, etc.
  - **Ortholinear or column-staggered arrangement**: Minimize the lateral finger movement that is provoked by traditional staggered key rows. Fingers primarily move straight up or down along columns, i.e. the directions they physically want to bend.
  - **Thumb cluster**: make extended use of both thumbs, which are strong and useful digits, rather than having both of them operate only a single key (the spacebar).
- Firmware
  - **Layers**: compensate for reduced number of keys by using layers (think Shift key on steroids)
  - **Tap-hold**: Instead of having dedicated hold keys (mods) and dedicated tap keys (letters, numbers. etc.), get more functionality by programming every key to have a tap output as well as a hold output.

When it comes to this specific layout, there are two main ergonomic features that I've prioritized in order to make it comfortable and fun for me to type on. I call them:

1. Home accessible keys
2. Hand-matching


### 1. Home accessible keys

**Home-accessible keys — can't think of a better name — are inputs that are quickly accessible by long-pressing a home-layer key if the user does not want to activate the layer that key is available on as a tap-function.**

As with many ergonomic layouts, the home layer — in fact, every layer — has home-row modifiers which are activated when a home-row key is long-pressed.

However, the top-row and bottom row of the alpha block also provide long-hold inputs. These are inputs which you _could_ access normally by finding them in their assigned layers, but they are also available via hold on the home-row for extra convenience. It often feels more effortless to make a quick 120ms+ hold with one finger than to have to make the key combo requires to access another layer.

The top row accessible keys are for tab-command in applications like web browsers. I also use them to control tabs in my IDE, my file explorer, my writing app… this is why they are home accessible! The first key opens the first tab, the second key opens the second tab, etc.

The bottom row accessible keys are for symbols I want to be able to access in the middle of typing without activating another layer.


### 2. Hand-matching

**Hand-matching is when each half of a layer corresponds to what a specific hand can best and most comfortably do when that layer is activated.**

Ergonomically speaking, it's not enough that each layer be specialized; each layer needs to be specialized _for each hand_. 

This plays out in three different ways:

1. **Frequently accessed keys and keys needed while typing are always on a layer half which is opposite the layer activation key.** In the same way that it is more comfortable to press shift with one hand and a letter with the opposite hand — rather than accomplish both tasks with a single hand — it is also more comfortable to press a layer key with one thumb and then the desired key on that layer with an opposite finger. I call that opposite hand the "primary hand." The "secondary hand" is the hand whose thumb activates the layer, because it is not as comfortable to type with that hand on that layer. For example, on layer 3, symbols are not distributed across both halves, the way we might expect with a number row, but are are clustered to the right. This is because layer three is activated with the left thumb, making the right hand the primary hand for that layer.
2. **Keys I frequently access while using the mouse are on left half of a layer activated by the left thumb.** These are "one-handed keys" meant to be useful during right-handed mouse use. Because this isn't the most ergonomic option when both hands are on the keyboard, all one-handed keys are also accessible on a two-handed layer. I choose which to use depending on context.
3. **Keys that are not frequently used and that are not used when typing are only on one-handed halves of the keyboard**. I suppose we could say that these are the only keys that are not "hand-matched."

The chart below summarizes the hand-matching logic of each layer:

| layer | activ. thumb | primary hand | secondary hand |
| ----- | ------------ | ------------ | -------------- |
| 1     | `Left`       | `R` numpad   | `L` nav (1h)   |
| 2     | `Right`      | `L` nav      | `R` media      |
| 3     | `Left`       | `R` symbols  | `L` Q-cmd (1h) |
| 4     | `Right`      | `L` symbols  | `R` f-keys     |

Two of the secondary halves are one-handed (1h) mouse-friendly halves, which leaves only two truly non-hand-matched halves: the media keys and the function keys. I just don't use them much…

##### QWERTY commands and hand-matching

One last thing about hand-matching. The left side of layer 3 is reserved for one-handed commands so that I can easily copy, paste, undo etc. while my hand is resting on a mouse.

It just so happens that QWERTY keyboards are already set up to do exactly this. Since many DVORAK typists are familiar with QWERTY shortcut positions, and may even have QWERTY legends on their keys (I know I do), these one-handed command keys are QWERTY, with a few additions.

## Legend

### All

- home-row: mods
- thumb-cluster: layers

### Home (Layer 0)

- alpha block:         DVORAK alpha block
- `HOLD` alpha TOP:     tab-control
- `HOLD` alpha BOTTOM:  frequent symbol

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|  '  |  ,  |  .  |  P  |  Y  |          |  F  |  G  |  C  |  R  |  L  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  A  |  O  |  E  |  U  |  I  |          |  D  |  H  |  T  |  N  |  S  |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|  ;  |  Q  |  J  |  K  |  X  |          |  B  |  M  |  W  |  V  |  Z  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  BRT  |  BSP  |  SFT  |          |  SPC  |  TAB  |  VOL  |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
| LG1 | LG2 | LG3 | LG4 | LG5 |          | LG6 | LG7 | LG8 | LG9 | LG0 |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI | APS |          | MSN | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|  !  |  ?  |  (  |  )  | ESC |          | CPL |  -  |  <  |  {  |  /  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  MO5  |  MO3  |  MO1  |          |  MO2  |  MO4  |  MO5  |      
      `-------'-------'-------'          `-------'-------'-------'      
```

### Layer 1

- alpha LEFT:  navigation cluster (one-handed)
- alpha RIGHT: number pad

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     | <<<*|  ^  | >>>*|     |          |  ,  |  7  |  8  |  9  |  0  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| CLP*|  <  |  v  |  >  |     |          |  .  |  4  |  5  |  6  | RET |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     | BCK*|     | FWD*|     |          |  *  |  1  |  2  |  3  |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |  XXX  |          |  SPL* |   0   |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |  XXX  |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- <<<: swipe left between fullscreen apps, `Option-Left-Arrow`
- \>>>: swipe right between fullscreen apps, `Option-Right-Arrow`
- CLP: Clipboard history, `Command-Option-Control-V`
- BCK: Back, `Command-Left-Bracket`
- FWD: Forward, `Command-RIght-Bracket`
- SPL: Spotlight search, `Command-Space`

### Layer 2

- alpha LEFT:  navigation cluster
- alpha RIGHT: media

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     | <<< |  ^  | >>> |     |          | MUT | VLD | VLU | BRD | BRU |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| CLP |  <  |  v  |  >  |     |          | REW | PLY | FFW | SKB | SKF |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     | LG[ |     | LG] |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |  XXX  |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |  XXX  |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

### Layer 3

- alpha LEFT:  QWERTY-commands (one-handed)
- alpha RIGHT: symbols 1

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
| LGQ | LGW | LGE | LGR | LGO |          |  (  |  &  |  *  |  `  |  )  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| LGA | LGS | LGD | LGF | LGN |          |  {  |  $  |  %  |  ^  |  }  |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
| LGZ | LGX | LGC | LGV | LGM |          |  [  |  !  |  @  |  #  |  ]  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |  XXX  |       |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |  XXX  |       |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

### Layer 4

- alpha LEFT: symbols 2
- alpha RIGHT: function keys

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|  <  |  >  |  …  |  \  |  |  |          |     | F7  | F8  | F9  | F12 |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  “  |  ”  |  «  |  »  |  €  |          |     | F4  | F5  | F6  | F11 |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----+
| en– | em— |  =  |  +  |  ≠  |          |     | F1  | F2  | F3  | F10 |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.
      |       |       |       |          |       |  XXX  |       |
      `-------'-------'-------'          `-------'-------'-------'

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |       |  XXX  |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

### Layer 5

- Controller
  - firmware: flash; reset
  - bluetooth: select profile; clear profile

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     |     | FLS | RST |     |          |     | RST | FLS |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| BTC | BT2 | BT1 | BT0 |     |          |     | BT0 | BT1 | BT2 | BTC |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  XXX  |       |       |          |       |       |  XXX  |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----+          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  XXX  |       |       |          |       |       |  XXX  |      
      `-------'-------'-------'          `-------'-------'-------'     
```