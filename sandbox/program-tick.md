```load-basic
cycle(100)

alive:
  walk(DOWN)
  walk(DOWN)

  walk(UP)
  walk(UP)
  
  walk(LEFT)
  walk(LEFT)
  
  walk(RIGHT)
  walk(RIGHT)
```

### Program Tick

What is a program tick? As your game runs, each update cycle is called a tick.

Basically one unit of movement / change. There are certain commands that will pause until next tick.

* walk
* follow
* jump
* idle
* shoot
* die

[Next Control Flow](control-flow.md)

---

[Back To Program Flow](program-flow.md) //
[Back To Start](start.md)
