```load-water
cycle(1)
dir = RIGHT
mode = GHOST
setTile(15) 
setColor(BLACK)
setCollision(mode)
jump(0, 5)

alive:
  walk(dir)
  every 20:
    dir = opp(dir)
  every 80:
    if mode == GHOST:
      mode = WALK
    else:
      mode = GHOST
    setCollision(mode) 
    
  events: 
    if event.THUD:
      talk(
        name(event.THUD) + ':' +
        tile(event.THUD) + ':' +
        color(event.THUD) + ':' +
        collision(event.THUD)
      )
      setTile(tile(event.THUD))
      setColor(color(event.THUD))
    if event.BLOCKED:
      talk(event.BLOCKED)
```

### Details

For getting or changing information about an object or terrain element there are details related commands.

[Next Scope](scope.md)

---

[Back To Vars](vars.md) //
[Back To Start](start.md)
