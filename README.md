# Tintin++ for DuneMUD

This is my personal script that I use when playing [DuneMUD[(https://dunemud.net).

There is nothing special here and it's probably not up to the best standards, but feel free to
snip whatever you want.

## Macros
I use "vim"-style macros `alt+h` for `west`, `alt+j`for `south` etc. but I've included macros for the keypad as well.

If you are using WSL+Windows terminal you need to hack it a bit to have the terminal send sequences that Tintin++ recognizes.
Open settings and in the lower left corner click the cog wheel, then add this to the actions section

```json
{ "command": { "action": "sendInput", "input": "\u001bOp" }, "keys": "numpad0" },
{ "command": { "action": "sendInput", "input": "\u001bOq" }, "keys": "numpad1" },
{ "command": { "action": "sendInput", "input": "\u001bOr" }, "keys": "numpad2" },
{ "command": { "action": "sendInput", "input": "\u001bOs" }, "keys": "numpad3" },
{ "command": { "action": "sendInput", "input": "\u001bOt" }, "keys": "numpad4" },
{ "command": { "action": "sendInput", "input": "\u001bOu" }, "keys": "numpad5" },
{ "command": { "action": "sendInput", "input": "\u001bOv" }, "keys": "numpad6" },
{ "command": { "action": "sendInput", "input": "\u001bOw" }, "keys": "numpad7" },
{ "command": { "action": "sendInput", "input": "\u001bOx" }, "keys": "numpad8" },
{ "command": { "action": "sendInput", "input": "\u001bOy" }, "keys": "numpad9" },
{ "command": { "action": "sendInput", "input": "\u001bOo" }, "keys": "numpad_divide" },
{ "command": { "action": "sendInput", "input": "\u001bOj" }, "keys": "numpad_multiply" },
{ "command": { "action": "sendInput", "input": "\u001bOm" }, "keys": "numpad_subtract" },
{ "command": { "action": "sendInput", "input": "\u001bOk" }, "keys": "numpad_add" },
{ "command": { "action": "sendInput", "input": "\u001bOn" }, "keys": "numpad_decimal" }
```