# Basic features

- 36-key layout (Microdox, Minidox, GergoPlex, perhaps a [split Planck](https://www.reddit.com/r/olkb/comments/vp9f5f/experimenting_with_a_bass_noise_amplifying_wood/?utm_source=share&utm_medium=ios_app&utm_name=iossmf))
    - 34 switches
    - 2 rotary encoders for media control and more (far left and far right of thumb cluster)
- DVORAK alpha layout
- Universal home-row mods
- Maximum inputs available on the default layer
- Easy one-handed commands for mouse users
- Mouse keys

If this keymap looks strange or messy to you, and you don't believe me when I say it is bliss to use, read the section below for a bit of explanation of my ergonomic logic.


# Ergonomic considerations
---

Pictura36 has some priorities which should be made clear at the outset. You'll notice that there are what look like strange redundancies — like some symbols existing both on layer 0 and on layer 2 — or needless complications — why are some Cmd combos on the home layer, some on the left side of layer 3, and why do either of them need to exist, let along both of them in separate places?

**This layout prioritizes my sense of ergonomics** over having tidy-looking layers or conforming to conventional keysets. The base layer is a great example of this: it can look like a messy hodgepodge of alphas, special commands, and mod-combos which even a full-size keyboard doesn't have dedicated keys for, let alone a 30% (like Cmd+1, Cmd+2, etc.)! The reason is simple: these are the inputs I use most! The goal is to make common inputs much more accessible from the default layer than with, say, the [Miryoku layout](https://github.com/manna-harbour/miryoku).

**Examples**: It might seem more tidy to put all symbols together on one layer, but it is in fact more practical to also place common symbols on the home layer as hold-inputs that don't require the use of both hands. Similarly, it might seem strange to have dedicated keys for Cmd+#, especially on the home layer, but the truth is I constantly use these to switch between tabs in some of my most used programs — such as my browser, IDE, and note-taking app.

Other features follow this same ergonomic logic. For example, you'll notice that the right side and left side of each layer contains completely unrelated inputs, even in cases where I could have made them more consistent. Again, although at first it may seem more intuitive and organized to have consistently within a layer, the truth is that layers that must be activated by holding down a key (all but layer 0), have very different ergonomic implications for each hand, since one of them has to hold the layer key down. 

**Example**: On layer 3, which is activated using the left thumb, mouse keys must be on the right, since they need to be pressed repeatedly or held down for an extended time without discomfort. One-handed commands, on the other hand, not only can more easily go on the left as keys which will only be quickly tapped, but moreover they *should* go on the left so that common commands can be accessed while the right hand is resting on a mouse or trackpad.


# Legends
---

## Legend position and layers

Top row = layer 0; top-left is tap, top-right is hold.

Home-row mods are in a brighter color than other L0 hold inputes; this is to indicate that they are in fact universal to all layers.

## Special icons

### L0: alphas, tab-control, common sybols, window management

<i class='fa fa-volume-down'></i> Volume up, volume down, mute

<i class='fa fa-th-large'></i> Mission control

<i class='fa fa-exchange'></i> Switch between two most recent apps (`Cmd + tab`)

### L1: navigation (L); number pad (R); media (C)

&#8647; Move to fullscreen app to the left (`Opt + left-arrow`)

&#8649; Move to fullscreen app to the right (`Opt + right-arrow`)

&#8678; Navigate backward (`Cmd + [`)

&#8680; Navigate forward (`Cmd + ]`)

<i class='fa fa-clipboard'></i> Show clipboard history*

<i class='fa fa-terminal'></i> Command palette (`Cmd + space`)**

<i class='kb kb-Multimedia-Play-Pause'></i> Play, pause, fast forward, rewind

---

_*Clipboard history pulled up via shortcut created in third party app Alfred._

_**This is a shorcut which is set up to call Spotlight, Alfred, Raycast, or some similar service._

### L3: one-handed commands (L); mouse (R)

&#9650; Move cursor up*

&#9679; Pramary click

&#11096; Secondary click

<i class='fa fa-angle-double-up'></i> Scroll up

<i class='fa fa-angle-double-down'></i> Scroll down

<i class='kb kb-Multimedia-FastForward-End'></i> Skip ahead, skip back

---

_*Cursor movements are currently controlled via shortcuts set up in the third party app Keymou._

### L5: controller

<i class='fa fa-rotate-right'></i> Reset controller

<i class='fa fa-flash'></i> Put controller in bootloader mode for flashing

<i class='fa fa-link'></i>2 Select bluetooth profile 2 and link with the corresponding device

<i class='fa fa-unlink'></i> Unlink with device assigned to selected bluetooth profile
