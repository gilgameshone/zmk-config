# Gilgamesh keymap

A 34-key keyboard layout on ZMK firmware that uses layers, tap-hold keys, and macros. The keys are laid out on a 3x5 grid + 2 thumb keys per hand. It is optimised to be used on Mac machines expecting a JIS keyboard (Kana input).

## Magic Sturdy mod

The base layer uses a modified Magic Sturdy for the alpha arrangement. The shifted characters are accessed by `SHFT` on tap that lasts for only one character. `Caps Word` can be accessed by tapping `SHFT` and `SPC` simultaneously. 

```
 ╭─────────────────────╮ ╭─────────────────────╮
 │  X   M   L   C   P  │ │  B   §   U   O   Q  │ 
 │  S   T   R   D   Y  | |  F   N   E   A   I  │ 
 │  V   K   J   G   W  │ │  Z   H  ',  ".  ?-  │ 
 ╰─────────╮  BKSP SPC │ │ SHFT  REP ╭─────────╯
           ╰───────────╯ ╰───────────╯
```

## Magic keys "§"

|     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Prev  | `A` | `B` | `C` | `D` | `E` | `F` | `G` | `H` | `I` | `J` | `K` | `L` | `M` | `N` | `O` | `P` |
| Magic | `O` | --  | `Y` | `Y` | `U` | --  | `Y` | --  | --  | --  | --  | `R` | `T` | --  | `A` | `Y` |

|     |     |     |     |     |     |     |     |     |     |     |     |     |     | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| Prev  | `Q` | `R` | `S` | `T` | `U` | `V` | `W` | `X` | `Y` | `Z` | `,` | `.` | `-` | 
| Magic | --  | `L` | --  | `M` | `E` | --  | --  | `T` | --  | --  | --  | --  | --  |


## other layers
### Num (hold BKSP)
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │  ?   [   ]   : C-F2 │ │  +   7   8   9   *  │ 
 │  &   (   )   ;   @  | |  -   4   5   6   /  │ 
 │  "   '   _   !   |  │ │  =   1   2   3   0  │ 
 ╰─────────╮           │ │ RET     ╭───────────╯
           ╰───────────╯ ╰─────────╯
```

### Sym (hold SPC)
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │                  #+ │ │  °   #   <   >   ^  │ 
 │                     | |  ~   %   {   }   `  │ 
 │                     │ │  §   ¥   $   £   €  │ 
 ╰─────────╮           │ │ RET     ╭───────────╯
           ╰───────────╯ ╰─────────╯
```

### Nav (hold REP)
```
 ╭─────────────────────╮ ╭─────────────────────╮
 │ Und Cut Cpy Pst Rdo │ │         Eis Kan     │ 
 │ ←   ↑   ↓   →       | |     Ctl Cmd Opt Sft │ 
 │ Hme PgD PgU End     │ │ Rwd Pse vDn vUp Mut │ 
 ╰─────────╮ ESC       │ │         ╭───────────╯
           ╰───────────╯ ╰─────────╯
```


### Ext (hold SHFT)
```
 ╭─────────────────────╮ ╭────────────────────────────╮
 │                     │ │  C-TAB TAB G-TAB A-TAB     │ 
 │                     | |  C-DEL DEL G-DEL A-DEL     │ 
 │                     │ │        Gogl gTrn defn Caps │ 
 ╰─────────╮           │ │         ╭──────────────── ─╯
           ╰───────────╯ ╰─────────╯
```
## Japanese JIS kana Tron arrangement


### Base
```
 ╭────────────────╮  ╭────────────────╮
 │　ら　る　こ　は　ょ │  │　き　の　く　あ　れ │ 
 │　た　と　か　て　も |  |　を　い　う　し　ん │ 
 │　ま　り　に　さ　な │  │　す　つ　、　。　っ │ 
 ╰─────────╮　⌫　R↑│  │　↓B　REP╭───────╯
           ╰──────╯  ╰────────╯
```
### Red R↑

```
 ╭────────────────╮   ╭────────────────╮
 │　ひ　そ　・　ゃ　ほ │   │　ぎ　げ　ぐ　あ　ゐ │ 
 │　ぬ　ね　ゅ　よ　ふ |   |　お　ぢ　ゔ　じ　ゑ │ 
 │　ぇ　ぉ　せ　ゆ　へ │   │　ず　づ　，　．　ゎ │ 
 ╰─────────╮　⌫　R↑│   │　⇅　REP╭────────╯
           ╰──────╯   ╰───────╯
```
### Blue ↓B

```
 ╭────────────────╮  ╭────────────────╮
 │　び　ぞ　ご　ば　ぼ │  │　え　け　め　む　ろ │ 
 │　だ　ど　が　で　ぶ |  |　お　ち　ー　み　や │ 
 │　ヵ　ヶ　ぜ　ざ　べ │  │　わ　ぃ　ぁ　　　ぅ │ 
 ╰─────────╮　⌫　⇅ │  │　↓B　REP╭───────╯
           ╰──────╯  ╰────────╯
```
### Purple ⇅

```
 ╭────────────────╮  ╭───────────────╮
 │　ぴ　　　　　ぱ　ぽ │  │  　　　　 　　　／│ 
 │　　　　　　　　　ぷ |  |　⎵ ひ　カ　Ｒ　r │ 
 │　　　　　　　　　ぺ │  │　　　↩ ；　：　？ │ 
 ╰─────────╮　⌫　⇅ │  │　⇅　REP╭───────╯
           ╰──────╯  ╰───────╯
```
