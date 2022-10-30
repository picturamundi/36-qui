## Ergonomic considerations

This isn't the place to explain at length yet again what are often cited as potential ergonomic advantages of programmable, tiny keyboards like the Microdox for touch-typists. I'll only briefly list this potential advantages below, and note that they need to be nuanced.

- Hardware 
  - **36-key layout**: Minimise wrist movement for touch-typists by placing all keys within immediate reach of fingers resting on the home row. Also makes it easier to type without ever looking at the keyboard — even for numbers, function keys, etc.
  - **Column-staggered arrangement**: Minimize the lateral finger movement that is provoked by traditional staggered key rows. Fingers move straight up or down along columns, i.e. the directions they physically want to bend.
  - **Thumb cluster**: make full use of both thumbs, which are strong and useful digits, rather than having both of them operate only a single key (the spacebar).
- Firmware
  - **Layers**: Compensate for reduced number of keys by using layers (think Shift key on steroids).
  - **Tap-hold**: Get more functionality out of each key by programming a tap output as well as a hold output, as opposed to having dedicated hold keys (e.g. mods) and dedicated tap keys (e.g. letters, numbers. etc.)

In reality, every one of these alternative keyboard features has pretty big disadvantages alongside the advantages. Take layers: they often simply replace the physical effort of reaching for keys with the physical effort of complicated key combos as well as the mental effort of keeping track of them.

In my experience, tiny keyboards work only if you can very carefully balance the pros and cons of layers, tap-holds, and so on, in order to get them to behave well in unison.

There are two main ergonomic features that I've prioritized in order to try and solve things like the layer problem, making it comfortable and fun for me to type with this layout. I call them:

1. Home accessible keys
2. Hand-matching


### 1. Home accessible keys

**Home-accessible keys are one of my solutions to the layer problem. It's what I call non-home layer inputs that are also made available on the home layer for easy non-repeat use via a long-press.**

As with many ergonomic layouts, the home layer — in fact, every layer — has home-row modifiers which are activated when a home-row key is long-pressed (held down for more than 120 milliseconds).

However, in this layout, the top-row and bottom row of the alpha block also give long-press inputs. They are all inputs which you _could_ access normally by finding them in their assigned layers, but which are also available via long-press on the home layer for extra convenience. It often feels more effortless to make a quick 120ms+ hold with one finger than to have to make the key combo requires to access another layer, provided the key doesn't need to repeat.

**Top row accessible keys**: tab-command in applications like web browsers. I also use them to control tabs in my IDE, my file explorer, my writing app, and more. The first key opens the first tab, the second key opens the second tab, etc.

**Bottom row accessible keys**: symbols I want to be able to access in the middle of typing without activating another layer.

Below is a map of hold-functions on the alpha block of the home layer. See the [legend](#legend) for more visuals.

```
          ,-----.-----.-----.-----.-----.  ,-----.-----.-----.-----.-----.
Tabs      | LG1 | LG2 | LG3 | LG4 | LG5 |  | LG6 | LG7 | LG8 | LG9 | LG0 |
          |-----+-----+-----+-----+-----|  |-----+-----+-----+-----+-----|
Mods      | SFT | CTL | ALT | GUI | APS |  | MSN | GUI | ALT | CTL | SFT |
          |-----+-----+-----+-----+-----|  |-----+-----+-----+-----+-----|
Symbols   |  !  |  ?  |  (  |  )  | ESC |  | CPL |  -  |  <  |  {  |  /  |
          `-----'-----'-----'-----'-----'  `-----'-----'-----'-----'-----'
```

It is rare to be able to access something like an angled bracket or Cmd-5 from the home layer of such a small keyboard, but this is a game changer for me when it comes to very frequently used inputs that don't fit on a regular alpha block.


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

#### QWERTY commands and hand-matching

One last thing about hand-matching. The left side of layer 3 is reserved for one-handed commands so that I can easily copy, paste, undo etc. while my hand is resting on a mouse.

It just so happens that QWERTY keyboards are already set up to do exactly this. Since many DVORAK typists are familiar with QWERTY shortcut positions, and may even have QWERTY legends on their keys (I know I do), these one-handed command keys are QWERTY, with a few additions.