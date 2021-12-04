```load-basic
cycle(100)

alive:
  idle()
  
  talk('down')
  walk(DOWN)
  walk(DOWN)

  talk('up')
  walk(UP)
  walk(UP)
  
  talk('left')
  walk(LEFT)
  walk(LEFT)
  
  talk('right')
  walk(RIGHT)
  walk(RIGHT)
```

### Program Tick

What is a program tick? As your game runs, each update cycle is called a tick. Crypto cafe uses a **fixed** number of updates per second.

Crypto Cafe runs at **25** ticks per second.

Basically one unit of movement / change. There are certain commands that will pause until next tick.

* walk
* follow
* jump
* idle
* shoot
* die

Try changing the value given to `cycle` to **10**. See how it effects the object.

[Next Control Flow](control-flow.md)

---

[Back To Program Flow](program-flow.md) //
[Back To Start](start.md)
