# Gilgamesh keymap

A 34-key keyboard layout on ZMK firmware that uses layers, tap-hold keys, and macros. The keys are laid out on a 3x5 grid + 2 thumb keys per hand. It is optimised to be used on Mac machines expecting a JIS keyboard (Kana input), and uses Alfred for some functions. 

## Magic Sturdy mod

The base layer uses a modified Magic Sturdy for the alpha arrangement. The shifted characters are accessed by `SHFT` on tap, a shift function that lasts for only one character. `Caps Word` can be accessed by tapping `SPC` and `REP` simultaneously. The repeat key, `REP`, helps to reduce single finger bigrams and improve typing comfort. 

```
                ╭───────☆───────╮
 ╭─────────────────────╮ ╭─────────────────────╮
 │  X   M   L   C   P  │ │  B   ★   U   O   Q  │ 
 │  S   T   R   D   Y  | |  F   N   E   A   I  │ 
 │  V   K   J   G   W  │ │  Z   H  ',  ".  ?-  │ 
 ╰─────────╮  BKSP SPC │ │ REP  SHFT ╭─────────╯
           ╰───────────╯ ╰───────────╯
                   ╰─CapsWord─╯
```

## Magic keys "★"
The magic key outputs the following when the previous key is pressed. It also reduces single finger bigrams and improves typing comfort.

|     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Prev  | `A` | `B` | `C` | `D` | `E` | `F` | `G` | `H` | `I` | `J` | `K` | `L` | `M` | `N` | `O` | `P` |
| Magic | `O` | --  | `Y` | `Y` | `U` | --  | `Y` | --  | --  | --  | --  | `R` | `T` | --  | `A` | `Y` |

|     |     |     |     |     |     |     |     |     |     |     |     |     |     | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| Prev  | `Q` | `R` | `S` | `T` | `U` | `V` | `W` | `X` | `Y` | `Z` | `,` | `.` | `-` | 
| Magic | --  | `L` | --  | `M` | `E` | --  | --  | `T` | --  | --  | --  | --  | --  |


The second magic key `☆` (Sorcery) can be accessed by pressing `★` and `C` at the same time. This transforms things like "us☆" into "the United States" or "para☆" into "paragraph" using Alfred for snippet expansion (this is not yet onboard the keyboard). 

## other layers
### Num (hold BKSP)
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │  !   [   ]   : C-F2 │ │  +   7   8   9   *  │ 
 │  &   (   )   ;   @  | |  -   4   5   6   /  │ 
 │  ?   _   "   '   |  │ │  =   1   2   3   .  │ 
 ╰─────────╮           │ │ RET  0  ╭───────────╯
           ╰───────────╯ ╰─────────╯
```

### Sym (hold SPC)

This layer has some realestate available. `aPst` here pastes without formatting. `Ynk` pulls from Alfred's kill list / clipboard. `Cpy` and `Pst` are duplicated here for use with one hand mouse use. 

```
 ╭─────────────────────────╮ ╭─────────────────────╮
 │            Cpy Pst aPst │ │  °   #   <   >   ^  │ 
 │      M-DEL     DEL Ynk  | |  ~   %   {   }   `  │ 
 │ Caps def   gTr Ggl      │ │  §   ¥   $   £   €  │ 
 ╰───────────╮             │ │         ╭───────────╯
             ╰─────────────╯ ╰─────────╯
```

### Nav (hold REP)

Nav has some available realestate, but the hold key to access it gets used heavily. `Rwd` uses Alfred to rewind the media player slightly. 
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │ Und Cut Cpy Pst Rdo │ │ Ssel    Eis Kan     │ 
 │ ←   ↑   ↓   →       | |     Ctl Cmd Opt Sft │ 
 │ Hme PgD PgU End     │ │ Rwd Pse vDn vUp Mut │ 
 ╰─────────╮ ESC  TAB  │ │         ╭───────────╯
           ╰───────────╯ ╰─────────╯
```
### Combos

Combo use has proliferated to reduce thumb-holding strain. Probably best view visually. 

Symetrical combos are:
Capsword,
Eisu,
Kana,
Magic 2 (Sorcery),
Hiragana,
Katakana.

One hand combos are: 
Tab,
Space,
Esc,
Up,
Left,
Home,
Backspace,
Return,
Down,
Right,
End.

Thumb combos simulate third thumb key (as it was not comfortable):
Function keys, 
and window manipulation.


## Japanese JIS kana Tron arrangement

### Base
```
 ╭────────────────╮  ╭────────────────╮
 │　ら　る　こ　は　ょ │  │　き　の　く　あ　れ │ 
 │　た　と　か　て　も |  |　を　い　う　し　ん │ 
 │　ま　り　に　さ　な │  │　す　つ　、　。　っ │ 
 ╰─────────╮　⌫　R↑│  │　↓B　   ╭───────╯
           ╰──────╯  ╰────────╯
```
### Red R↑

```
 ╭────────────────╮   ╭────────────────╮
 │　ひ　そ　・　ゃ　ほ │   │　ぎ　げ　ぐ　あ　ゐ │ 
 │　ぬ　ね　ゅ　よ　ふ |   |　お　ぢ　ゔ　じ　ゑ │ 
 │　ぇ　ぉ　せ　ゆ　へ │   │　ず　づ　，　．　ゎ │ 
 ╰─────────╮　⌫　R↑│   │　⇅　   ╭────────╯
           ╰──────╯   ╰───────╯
```
### Blue ↓B

```
 ╭────────────────╮  ╭────────────────╮
 │　び　ぞ　ご　ば　ぼ │  │　え　け　め　む　ろ │ 
 │　だ　ど　が　で　ぶ |  |　お　ち　ー　み　や │ 
 │　ヵ　ヶ　ぜ　ざ　べ │  │　わ　ぃ　ぁ　　　ぅ │ 
 ╰─────────╮　⌫　⇅ │  │　↓B　   ╭───────╯
           ╰──────╯  ╰────────╯
```
### Purple ⇅

```
 ╭────────────────╮  ╭───────────────╮
 │　ぴ　　　　　ぱ　ぽ │  │  　　　　 　　　 │ 
 │　　　　　　　　　ぷ |  |　             │ 
 │　　　　　　　　　ぺ │  │　　　          │ 
 ╰─────────╮　⌫　⇅ │  │　⇅　   ╭───────╯
           ╰──────╯  ╰───────╯
```
#### key position reference 
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │  0   1   2   3   4  │ │  5   6   7   8   9  │ 
 │  10  11  12  13  14 | |  15  16  17  18  19 │ 
 │  20  21  22  23  24 │ │  25  26  27  28  29 │ 
 ╰─────────╮    30  31 │ │  32  33   ╭─────────╯
           ╰───────────╯ ╰───────────╯
```
