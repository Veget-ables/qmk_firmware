# The Default Helix Layout
## Layout

### Qwerty

```
 ,-----------------------------------------.             ,-----------------------------------------.
 |   `  |   1  |   2  |   3  |   4  |   5  |             |   6  |   7  |   8  |   9  |   0  |Delete|
 |------+------+------+------+------+------|             |------+------+------+------+------+------|
 | Tab  |   Q  |   W  |   E  |   R  |   T  |             |   Y  |   U  |   I  |   O  |   P  | Bksp |
 |------+------+------+------+------+------|             |------+------+------+------+------+------|
 | Tab  |   A  |   S  |   D  |   F  |   G  |             |   H  |   J  |   K  |   L  |  Up  | Bksp |
 |------+------+------+------+------+------+------+------+------+------+------+------+------+------|
 | Shift|   Z  |   X  |   C  |   V  |   B  | EISU | KANA |   N  |   M  |   C  | Left | Down |Right |
 |------+------+------+------+------+------+------+------+------+------+------+------+------+------|
 | Ctrl | Alt  | GUI  | Shift| Shift|Lower |Space |Enter |Raise | Shift| Shift|   ,  |   .  |  Alt |
 `-------------------------------------------------------------------------------------------------'
 
  ```

## Customize

see `qmk_firmware/keyboards/helix/rev2/keymaps/default/rules.mk`

```
# Helix keyboard customize
# you can edit follows 7 Variables
#  jp: 以下の7つの変数を必要に応じて編集します。
HELIX_ROWS = 5              # Helix Rows is 4 or 5
OLED_ENABLE = no            # OLED_ENABLE
LOCAL_GLCDFONT = no         # use each keymaps "helixfont.h" insted of "common/glcdfont.c"
LED_BACK_ENABLE = no        # LED backlight (Enable WS2812 RGB underlight.)
LED_UNDERGLOW_ENABLE = no   # LED underglow (Enable WS2812 RGB underlight.)
LED_ANIMATIONS = yes        # LED animations
IOS_DEVICE_ENABLE = no      # connect to IOS device (iPad,iPhone)

```
## Compile

go to qmk top directory.
```
$ cd qmk_firmware
```

build
```
$ make helix:default
```

flash to keyboard
```
$ make helix:default:avrdude
```

## Link
* more detail wrote in Japanese [helix/Doc/firmware_jp.md](https://github.com/MakotoKurauchi/helix/blob/master/Doc/firmware_jp.md)
* [Helix top](https://github.com/MakotoKurauchi/helix)

