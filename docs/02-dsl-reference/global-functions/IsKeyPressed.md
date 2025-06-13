---
description: Check if a keyboard key is currently pressed.
sidebar_class_name: hidden
---

# IsKeyPressed

> **_This function was added in DSL 1_**

## Description

Check if a key is currently pressed.

`key` should be given as a DirectInput keyboard scan code name (listed below), but can also be given as a directly as a number.

If a `controller` is specified, a game input device will be used instead of the DSL keyboard. This is a good way to respect when other scripts disable controls. Using controller 0 also ensures that the player is actually using a keyboard to play rather than an xbox controller.

```lua
function IsKeyPressed(key, controller) --[[ ... ]] end
```

## Parameters

- `key`: _`string`_ - The name of the key to check.
- `controller?`: _`0|1|2|3`_ - (Optional) The controller to check the key on. Defaults to `0`, which is the keyboard.

## Return Values

- `pressed`: _`boolean`_ - Returns _`true`_ if the key is currently pressed, otherwise _`false`_.

## Versions

- **DSL4** - DirectInput keyboard scan codes are now used, but virtual key code names will still be converted for legacy support.
- **DSL5** - Keys are also reported as pressed when they are being pressed, and no longer when they are being released.
- **DSL6** - The optional `controller` argument was added.

## Example

Check if the 'W' key is currently pressed and print a message.

```lua
function main()
  local key = 'W'
  while true do
    -- highlight-next-line
    if IsKeyPressed(key) then
      DrawTextInline(key .. ' key is currently pressed!', 0, 1)
    end
    Wait(0)
  end
end
```

## DirectInput Keyboard Scan Code Names

```plaintext
ESCAPE
1
2
3
4
5
6
7
8
9
0
MINUS
EQUALS
BACK
TAB
Q
W
E
R
T
Y
U
I
O
P
LBRACKET
RBRACKET
RETURN
LCONTROL
A
S
D
F
G
H
J
K
L
SEMICOLON
APOSTROPHE
GRAVE
LSHIFT
BACKSLASH
Z
X
C
V
B
N
M
COMMA
PERIOD
SLASH
RSHIFT
MULTIPLY
LMENU
SPACE
CAPITAL
F1
F2
F3
F4
F5
F6
F7
F8
F9
F10
NUMLOCK
SCROLL
NUMPAD7
NUMPAD8
NUMPAD9
SUBTRACT
NUMPAD4
NUMPAD5
NUMPAD6
ADD
NUMPAD1
NUMPAD2
NUMPAD3
NUMPAD0
DECIMAL
OEM_102
F11
F12
F13
F14
F15
KANA
ABNT_C1
CONVERT
NOCONVERT
YEN
ABNT_C2
NUMPADEQUALS
PREVTRACK
AT
COLON
UNDERLINE
KANJI
STOP
AX
UNLABELED
NEXTTRACK
NUMPADENTER
RCONTROL
MUTE
CALCULATOR
PLAYPAUSE
MEDIASTOP
VOLUMEDOWN
VOLUMEUP
WEBHOME
NUMPADCOMMA
DIVIDE
SYSRQ
RMENU
PAUSE
HOME
UP
PRIOR
LEFT
RIGHT
END
DOWN
NEXT
INSERT
DELETE
LWIN
RWIN
APPS
POWER
SLEEP
WAKE
WEBSEARCH
WEBFAVORITES
WEBREFRESH
WEBSTOP
WEBFORWARD
WEBBACK
MYCOMPUTER
MAIL
MEDIASELECT
BACKSPACE
NUMPADSTAR
LALT
CAPSLOCK
NUMPADMINUS
NUMPADPLUS
NUMPADPERIOD
NUMPADSLASH
RALT
UPARROW
PGUP
LEFTARROW
RIGHTARROW
DOWNARROW
PGDN
CIRCUMFLEX
```

## See Also

- DSL
  - [`IsKeyBeingPressed`](./IsKeyBeingPressed) - Check if a key was just pressed.
  - [`IsKeyBeingReleased`](./IsKeyBeingReleased) - Check if a key was just released.
  - [`IsKeyValid`](./IsKeyValid) - Check if a key is valid without raising an error.
