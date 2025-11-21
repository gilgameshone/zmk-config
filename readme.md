# Gilgamesh keymap

A 34-key keyboard layout on ZMK firmware that uses layers, tap-hold keys, and macros. The keys are laid out on a 3x5 grid + 2 thumb keys per hand. It is optimised to be used on Mac machines expecting a JIS keyboard (Kana input), and uses Alfred for some functions. 

## Magic Sturdy mod

The base layer uses a modified Magic Sturdy for the alpha arrangement. The shifted characters are accessed by `⇧` on tap, a shift function that lasts for only one character. `Caps Word` can be accessed by tapping `␣` and `®` simultaneously. The repeat key, `®`, helps to reduce single finger bigrams and improve typing comfort. 

```
                ╭───────☆───────╮
 ╭─────────────────────╮ ╭─────────────────────╮
 │  X   M   L   C   P  │ │  B   ★   U   O   Q  │ 
 │  S   T   R   D   Y  | |  F   N   E   A   I  │ 
 │  V   K   J   G   W  │ │  Z   H  ',  ".  ?-  │ 
 ╰───────────╮  ⌫  ␣  │ │  ®   ⇧  ╭───────────╯
             ╰─────────╯ ╰─────────╯
                   ╰CapsWord╯
```
```
® repeat
⇧ one shot shift
␣ space
⌫ backspace
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
 │  &   (   )   ;   #  | |  -   4   5   6   /  │ 
 │  ?   _   %   @   |  │ │  =   1   2   3   .  │ 
 ╰─────────╮           │ │ RET  0  ╭───────────╯
           ╰───────────╯ ╰─────────╯
```

This layer can also be accessed by pressing `BKSP` and `SFT`, which turns on a numword layer that will cancel after space or return are pressed. 


### Sym (hold SPC)

This layer has some realestate available. `aPst` here pastes without formatting. `Ynk` pulls from Alfred's kill list / clipboard. `Cpy` and `Pst` are duplicated here for use with one hand mouse use. 

```
 ╭─────────────────────────╮ ╭─────────────────────╮
 │                         │ │  °   #   <   >   ^  │ 
 │                 DEL Ynk | |  ~   %   {   }   `  │ 
 │ Caps def   gTr Ggl      │ │  §   ¥   $   £   €  │ 
 ╰───────────╮             │ │         ╭───────────╯
             ╰─────────────╯ ╰─────────╯
```

### Nav (hold REP)

Nav has some available realestate, but the hold key to access it gets used heavily. `Rwd` uses Alfred to rewind the media player slightly. 
```
 ╭─────────────────────╮ ╭───────────────────────╮
 │                     │ │ Ssel  CTL CMD OPT SFT │ 
 │ ←   ↑   ↓   →       | | Globe Ctl Cmd Opt Sft │ 
 │ Hme PgD PgU End     │ │ Rwd   Pse vDn vUp Mut │ 
 ╰─────────╮ ESC  TAB  │ │         ╭─────────────╯
           ╰───────────╯ ╰─────────╯
```
CMD (and the like) are sticky modifiers. 

### Combos

Combo use has proliferated to reduce thumb-holding strain. Probably best view visually. Currently, I am experimenting with 'vertical' combos, one's that should have less of an impact when using rolling motions when typing. 

```
xs = esc ⎋
mt = copy ⌘C
lr = paste ⌘V
cd = eisu 英数
py = hiragana ひらがな
sv = tab ↹ 
tk = space 
rj = left ← 
dg = up ↑
dy = delete word forward ⌥ ⌦
yw = home ⇱
cp = undo ⌘Z


bf = katakana カタカナ
★n = kana かな
fn = backspace word ⌥ ⌫
fz = end ⇲
nh = down ↓
e, = right →
a. = return ⏎
i- = select all ⌘a
oa = save ⌘s
ue = apostrophe '
qi = double quotation mark "

␣® = capsword
⌫⇧ = numword

★c = sorcery 
dn = select word

qi- = ble layer
⌫␣ = fn layer 
®⇧ = meh layer
```



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
 │　ぴ　　　　　ぱ　ぽ │  │　　　　　　　　　│ 
 │　全角　　　　　　ぷ |  |　　　　　　　　　│ 
 │　　　　　　　　　ぺ │  │　　　　　　　　　│ 
 ╰─────────╮　⌫　⇅ │  │　⇅　　　╭───────╯
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
![Gilgamesh keymap drawer image](https://caksoylar.github.io/keymap-drawer?keymap_yaml=H4sIAAAAAAAC_-0d23LiuPJ9vkJP690KUxUgk9ubsYVxMLbjSybJ1BRFApNJDQksl92T2prfOH-zP7NfciRZN4NJiOVs4OBUpWh1S62W1C21WkgMe0-j-ewU_PX7w4_uj8HTzag36Z-Cb4PJ5H7anYxmvdmg__PDsPc0mExPPwDw0Lu7v-1OZ_NJ_wmnP4Iv2i8Pd93_aBVAgAcGDBlwy4AxAhoV4MaNkGLmjDRCwPlXwu8j-AsJhHJ8PwVO2GpGPxEaUDTJPAORlpB1Z5k6AQGlWrG9RO0Dk1KNKHAY-Yp-NqXsLskWyNk4lwGACZcgq44e0Cl1QT47wbJG4bZeUHKbfp4tMrsDVsIs_Dbb04ezPWt-v4el51J9pp_XUtHW80UI91-vO23Qsk0Qh7oFf-UQaMOrCkgl8X_D0wMTGF6nowPdNYEDwxBELd397Tck4BQxxNWBXFyPCEe948MgRBDiqC4p4mV7JmFsBVCPYFCUtLVE2qgQMTu2G4eEYeyaqPmGF8ACZAwdPWwRtucxDCPbc4mk-K-jB20qOrO2Rjv0icY8zh_kJoW-bkBCmD5xgvYLmii6k8F40JtpUmZkrHYzStj0_sC58bzQHZ5KFf3z378rYPY0HpyC2aT3OJUr2xRa9Ea8t6kP_k1a2S-b0S948S6ttdTKsl-2xFqH22etQamVpbXuprXOt89aYamVpbXuprWOts9a9VIrS2vdTWudbZ-1dkqtLK11N611sn3W6pRaWVrrblprf_us9arUytJa_4_7JfkmQ19LDHSwfQYal4pYGuhuLqe97bNWr9TK0lp301pvS-e31MqyX7bEWu9Kay21suyXjduq3t3Rreq4NNBSEct-2TgDHY-xgc4mo8fuTW86YBd7ct088MjtheLvbGRwpFcaXubbUJCpmZTNfRWDCnlCL800I-DrAXSjFgztUEEuS6FsO11W7sc1ObQUaq-Trmjp4euYUCnT11xgxzY8x3MJSwIhnl9V9PdcoWWhcoMihdo_K5TtPKvlaxvaPhmHwLZaRak5XLPsooiCwwGRyfQcRw8UBDEVyl6pKuWZQuWOslLaCrVfKpSNlSd-lQG_LmbiX3VjUuFy37PL5GvYZg32NdfVhbuBxD1YuCBIcJNBP7kjOLu__fG0RL4Zzgcr6FlOCS_DrxdHZ92GTW4KI-jaY5DFoYbOIS_3cH8i_Ym61kCzlvKko_teGAWe34L0EqYXQZWFZek6J7vG-RJHKuIKvi5iFIdkLSbcI9sxVeS0XaSMro4F1J2qNOvhwTH5MJliEAUO8kGMc9d_mPgBaOWJlGc9vah-qCswknzfxZHMfbeaWXf-CWjBVqhF5-eXGja-McHWDrVUUk8lG5yaq9aVzopye2ABPGQveY19XP6K0v7RmltNMkuP55PxMHtuJ6W-D4b9taZ7tIKwuFCuJlzwLsr3qEEBw7VyhlbmvGTAKk3Nfm5ANirLTtmYlbZAK9YUgxi5xK4SkeGl4egdMqsqDniWT6Y8UMfJQIVo6rfDtpqEq8IFKjzFuxUqXFbO1eZ1WnMu4lTyzNZe1I4vWmFrkpqHnelH5FyAfYXlf1GlFN09eB7rTtJPTkx35WRdjbkXJkCnrVt2W29zXy2QEarbooVd-de11p3MVeWlpeiZdScpxZYe0kjf1pQjqphN2lPxPa2Ms9OuiN-yK4zZMKfJO3w2y88jMxz5rp0N30vvcPVh9xz7QFpe236dE_k4f5BCBmEXXjrrTWUkNxkslCKD36wxNJ4neR73SIDHAjzhIJqoUXO_ylIgv00wcNBazhOBnMCaI9hEHCT-mqjqQICfBHgo2GAvNC1AMgQsA_H6eMo8FzWFEuzbPuQJsmiIyqoCrAmwLsB9aTJfewTJ4xCQPeZCxnP69MCGFoHvdW7c9oHrGO21NR5v2LQUxonSaWshTbwM7Z2aZ7thShgSAErL5wfugsROIzDSmGAJYwX6BdQ28EAXPz-YkvQKumnRTccJNOWl9VWq_4qp8bH3B53myLN-1xVAPi_pp0E_LypkJ8PycPhTBTi6a5EJrgvtMHH3um3dxZE4TKoy80WeGXtbMBagKcBAgLkfhMHvKzLYim3O2WFzAXkukUrU8jrsTQrfArEvYNNlb1a45hrVthBqsgcaUlbfJ2_u-T7Lc-E5gi1O8Po6cQSpRDA02ENUeiPHYIo1K_9mJWNznHvDkUTDGoFutGEk4mPUacd4lfBw0eHmdJSdCili7WItV4jrZJ4w5xSYSrgckv3X9ocvxxuojEunt_m7cMVZiHoYOisUUXj4Jj_Dt4jhrNph5GZIxJPtnSNgKu5c_OumyLMi5J8q4i8Fr3Nzyj7TKEwvCw8qq60Z-Q8U1z76S2JRxbyzWyn2dWGZXc6oXtYJX34RV9qJSuCxSL8gPRYK38jI-eWvdb8Aobz1LPwksYC9a-LYy4kLaXHiL3wvIsHxWxxC5mf2NqcuK3VBZUAXA-VrDCDpcROu81KIyEX3IVfqJ87LAoONOuJfsbFY8DTy81-xtVDm-5J_hNXC0H0RUugPvt0_ioDCHR55KTka3Q2114UpCvkGSvFfE-BKX1-cd2r5D3NeOz1-mz9uRmTQD42ABQuaJwyo7nOoyqHau8f6QiF38xMDDhlwxIDjDQzf-XocQmR_UOct4D1bYwDTyObBc-5AIQp4I84PGxEwnGBn7qmkuq-8tpPZHY3k9zC0g9QvhTBsPRNby8RWM7H72o6O_5_3fN7vDL7vgUsWmsWJjpxYxyEjGf0NPKEngoWylJGcCOSEuWW32YjQF3IL2nLiTE5YcuLzln2VIhlE31jzqPt29HAzmp5--AjGp-BLvVoB9Rre1v7Avwh12xtPu3-OJn2N0fcRvUrpyBti6BpC1ykaGQtFn1RAFf3XTigFrV6UUkMFaqwAiQNT_CHCH1F8chZACUiwGhOMuH1yqSNEPJaJS0VZXeRMR6qLlcIHOQm6Wpdqin2GlQUzvc8uwy_JJYocS0WS_Zoohyo5pCTiJBMHXLCsMnnxOY-EPmDihoaMrkklyK8oSVJXUedUWTNx5EEiMTS-dcF6pQKO-PgnR3asRAUcCwo5wmMUXD8rRY5BzmTpjmVK-8P_AD70YMkGbgAA)
