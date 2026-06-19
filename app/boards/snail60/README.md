# snail60

The snail60 is a hotswap 60% keyboard.

## Building snail60 ZMK firmware

ZMK Studio support over USB is enabled by default for this board.

```
west build -p -b snail60
west flash
```

The default keymap includes `&studio_unlock` on the Fn layer so Studio can make
changes after the keyboard is unlocked.

## Physical layout

```
["0,0","0,1","0,2","0,3","0,4","0,5","0,6","0,7","0,8","0,9","0,10","0,11","0,12",{w:2},"0,13"],
[{w:1.5},"1,0","1,1","1,2","1,3","1,4","1,5","1,6","1,7","1,8","1,9","1,10","1,11","1,12",{w:1.5},"1,13"],
[{w:1.75},"2,0","2,1","2,2","2,3","2,4","2,5","2,6","2,7","2,8","2,9","2,10","2,11",{w:2.25},"2,13"],
[{w:2.25},"3,0","3,1","3,2","3,3","3,4","3,5","3,6","3,7","3,8","3,9","3,10",{w:2.75},"3,13"],
[{w:1.25},"4,0",{w:1.25},"4,1",{w:1.25},"4,2",{a:7,w:6.25},"4,5",{a:4,w:1.25},"4,9",{w:1.25},"4,10",{w:1.25},"4,12",{w:1.25},"4,13"]
```

## Default layer

```
["Esc\n`","!\n1","@\n2","#\n3","$\n4","%\n5","^\n6","&\n7","*\n8","(\n9",")\n0","_\n-","+\n=",{w:2},"Backspace"],
[{w:1.5},"Tab","Q","W","E","R","T","Y","U","I","O","P","{\n[","}\n]",{w:1.5},"Delete"],
[{w:1.75},"Caps Lock","A","S","D","F","G","H","J","K","L",":\n;","\"\n'",{w:2.25},"Enter"],
[{w:2.25},"Shift","Z","X","C","V","B","N","M","<\n,",">\n.","?\n/",{w:2.75},"Shift"],
[{w:1.25},"Ctrl",{w:1.25},"Win",{w:1.25},"Alt",{a:7,w:6.25},"",{a:4,w:1.25},"Alt",{w:1.25},"Menu",{w:1.25},"Ctrl",{w:1.25},"Fn"]
```

## Fn layer

```
["~\n`","F1","F2","F3","F4","F5","F6","F7","F8","F9","F10","F11","F12",{w:2},"Soft Off"],
[{w:1.5},"BT Clear","","Up","","Prev","Vol+","Bright+","PrtSc","ScrLk","Pause","","Backlight-","Backlight+",{w:1.5},"|\n\\"],
[{w:1.75},"BT 0","Left","Down","Right","Next","Vol-","Bright-","Ins","Home","PgUp","","",{w:2.25},"Boot"],
[{w:2.25},"BT 1","BT 2","BT 3","BT 4","Play/Pause","Mute","","Delete","End","PgDn","Up",{w:2.75},"Studio Unlock"],
[{w:1.25},"",{w:1.25},"",{w:1.25},"",{a:7,w:6.25},"Backlight Toggle",{a:4,w:1.25},"Left",{w:1.25},"Down",{w:1.25},"Right",{w:1.25},"Fn"]
```
