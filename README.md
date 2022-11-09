# Pictura Keyboard Layout Manual

Pictura is a ergonomic keyboard layout compatible with devices running the ZMK keyboard firmware.

For all information on how ZMK works, how to use this layout, how to edit it, and so on, see the official [ZMK documentation](https://zmk.dev/docs).

<!--While this file briefly summarizes the [main features](#at-a-glance) of the layout and provides a [visual legend](#legend) for each layer, a more in-depth explanation of its ergonomic design can be found at [picturamundi.com/type](https://picturamundi.com/type.html).-->


## At a glance…

A couple of things you should know before using this firmware for yourself:

- It's a 36-key layout made with a [Microdox](https://boardsource.xyz/store/5f2e7e4a2902de7151494f92) in mind. Since the Microdox has has a very retracted thumb-cluster, I treat the innermost key as the primary thumb key. It might be best to edit the keymap and swap this inner key with the middle thumb key for something like a Corne.
![microdox](/images/microdox-bud.svg)
_Microdox_

- For commands with no dedicated ZMK key-code (e.g. navigate backward and forward on webpages), I'm using shortcuts combos that work on my personal machine, but they may have to be customized for other devices. See the [layout legend](#legend) below if ever you're confused about what these shortcuts in the keymap are supposed to actually do.

How does this layout compare to the popular 36-key [Miryoku layout](https://github.com/manna-harbour/miryoku/tree/master/docs/reference)? With the understanding that this is a much less fully-featured project which was designed with only my own personal use in mind, here are nonetheless the key advantages for me: 
  - Tap-Shift for less finger strain when typing, with the option of a tradition hold-shift in the form of a home-row mod
  - Tab-control on home-layer… in fact in general [there's just more that's accessible on the home layer](#1-home-accessible-keys)
  - One-handed layers for mouse-friendly use, with inputs that are also available on two-handed layers for more ergonomic use when both hands are on the keyboard
  - DVORAK alphas with optional [QWERTY command shortcuts](#qwerty-commands-and-hand-matching)
  - Eventually, when I get around to installing rotary encoders on my Microdox, the plan is to support them with much more practical media inputs.

## Legend

Anything marked as `HOLD` only outputs the specified keypress when the key is held down for a longer amount of time than a regular tap, generally a minimum 120 milliseconds.

### All layers

- `HOLD` home-row: mods
- `HOLD` thumb-cluster: layers

### Layer 0 (Home)

- **alpha block**:         DVORAK
- `HOLD` **alpha top row**:     tab-control
- `HOLD` **alpha bottom row**:  frequent symbol

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|  '  |  ,  |  .  |  P  |  Y  |          |  F  |  G  |  C  |  R  |  L  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  A  |  O  |  E  |  U  |  I  |          |  D  |  H  |  T  |  N  |  S  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  ;  |  Q  |  J  |  K  |  X  |          |  B  |  M  |  W  |  V  |  Z  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  BRT  |  BSP  |  SFT  |          |  SPC  |  TAB  |  VOL  |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|  T1 |  T2 |  T3 |  T4 |  T5 |          |  T6 |  T7 |  T8 |  T9 |  T0 |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI | APS |          | MSN | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  !  |  ?  |  (  |  )  | ESC |          | CPL |  -  |  <  |  {  |  /  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  MO5  |  MO3  |  MO1  |          |  MO2  |  MO4  |  MO5  |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- Home-row mods imitate the order of mods on a macbook.
  - GUI: Command in macOS, windows key in Windows
  - ALT: Option in macOS
- `T1`, `T2` etc. : Select tab 1, select tab 2, etc. `Cmd-1`, `Cmd-2` etc. in macOS.
  - T9 selects the last tab in many browsers and some other applications.
  - T0 sets the zoom to 100% in some applications (Preview.app, for example).
- For hold inputs, the innermost keys of the bottom two rows comprise a separate section of their own. I think of it as a my home-layer navigation cluster:
  - APS: Uses the MacOS App Switcher to switch to the previous application. You can achieve the same thing with `Cmd-Tab`; this option is mouse friendly since it only requires the left hand, but is only practical for switching to the most recent app on the app switcher.
  - MSN: Mission control on MacOS (`Opt-Up`)
  - CPL: Caps Lock
- `MO1` etc. : Activate layer 1 when pressed down


### Layer 1

- **Left**:  navigation cluster (one-handed)
- **Right**: number pad

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     | <<< |  ^  | >>> |     |          |  ,  |  7  |  8  |  9  |  0  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| CLP |  <  |  v  |  >  |     |          |  .  |  4  |  5  |  6  | RET |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     | <== |     | ==> |     |          |  *  |  1  |  2  |  3  |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |  XXX  |          |  SPL  |   0   |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |  XXX  |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- `<` `>` `^` `v` : left, right, up, down
- `<<<` `>>>`: swipe left and right between fullscreen apps in macOS, `Opt-left` and `Opt-right`
- `CLP`: Clipboard history — this is a shortcut configured in a third party app, `Cmd-Opt-Ctrl-V`
    `<==`: Back, `Cmd-leftBracket`
- `==>`: Forward, `Cmd-rightBracket`
- `SPL`: Spotlight search, `Cmd-Space` — the goal here is to reproduce similar thumb movements to what one would make hitting `Cmd-Space` on a mac

### Layer 2

- **Left**:  navigation cluster (two-handed use)
- **Right**: media

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     | <<< |  ^  | >>> |     |          |  << |  ⏵︎  |  >> | ⏐<< | >>| |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| CLP |  <  |  v  |  >  |     |          | MUT | VL- | VL+ | BR- | BR+ |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     | <== |     | ==> |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |  XXX  |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |  XXX  |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- `MUT`: Mute
- `VL`: Volume
- `BR`: Brightness


### Layer 3

- **Left**:  QWERTY-commands (one-handed)
- **Right**: symbols 1

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
| C-Q | C-W | C-E | C-R | C-O |          |  (  |  &  |  *  |  `  |  )  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| C-A | C-S | C-D | C-F | C-N |          |  {  |  $  |  %  |  ^  |  }  |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| C-Z | C-X | C-C | C-V | C-M |          |  [  |  !  |  @  |  #  |  ]  |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |  XXX  |       |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| SFT | CTL | ALT | GUI |     |          |     | GUI | ALT | CTL | SFT |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |  XXX  |       |          |       |       |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- `C-Q`, `C-W`, etc. : Cmd-Q, Cmd-W etc. All but the innermost column are QWERTY commands. The inner column doesn't correspond to QWERTY, but instead pulls frequently used commands which, in QWERTY, are under to right hand (O, N, and M).


### Layer 4

- **Left**: symbols 2
- **Right**: function keys

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|  <  |  |  |  \  |  /  |  >  |          |     | F7  | F8  | F9  | F10 |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|  “  |  ”  |  «  |  »  |  €  |          |     | F4  | F5  | F6  | F11 |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| em– | en— |  -  |  +  |  =  |          |     | F1  | F2  | F3  | F12 |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.
      |       |       |       |          |       |  XXX  |       |
      `-------'-------'-------'          `-------'-------'-------'

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |       |       |       |          |       |  XXX  |       |      
      `-------'-------'-------'          `-------'-------'-------'      
```

- `€`: in macOS `Opt-Sft-2`
- `en–`: en-dash `Opt-Dash`
- `em-`: em-dash `Opt-Sft-Dash`

### Layer 5

Controller commands

```
,-----.-----.-----.-----.-----.   TAP    ,-----.-----.-----.-----.-----.
|     |     | FLS | RST |     |          |     | RST | FLS |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
| BTC | BT2 | BT1 | BT0 |     |          |     | BT0 | BT1 | BT2 | BTC |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  XXX  |       |       |          |       |       |  XXX  |      
      `-------'-------'-------'          `-------'-------'-------'      

,-----.-----.-----.-----.-----.   HOLD   ,-----.-----.-----.-----.-----.
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
|-----+-----+-----+-----+-----|          |-----+-----+-----+-----+-----|
|     |     |     |     |     |          |     |     |     |     |     |
`-----'-----'-----'-----'-----'          `-----'-----'-----'-----'-----'
      ,-------.-------.-------.          ,-------.-------.-------.      
      |  XXX  |       |       |          |       |       |  XXX  |      
      `-------'-------'-------'          `-------'-------'-------'     
```

  - Firmware
    - `FLS` Flash (bootloader mode)
    - `RST` Reset 
  - Bluetooth
    - `BT0` etc. Select profile 
    - `BTC` Clear profile