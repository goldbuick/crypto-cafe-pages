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

For getting or changing information about an object or terrain element there are detail commands.

##### Names
 - `name(event.THUD)` returns the name of the given element 
 - `match(event.THUD, 'car')` returns true if the given element matches the name
 - `player(event.THUD)` returns true if the given element is named player 
 - `bullet(event.THUD)` returns true if the given element is named bullet **OR** collision is **BULLET**

##### Appearance
 - `tile(event.THUD)` tile is the sprite used to draw the game element
 - `color(event.THUD)` color is the color of the sprite used to draw the game element

##### Stats
 - `light(event.THUD)` on dark boards, this controls if the element emits light
 - `collision(event.THUD)` collision controls how objects can move around boards
 - `pushable(event.THUD)` tells wether an object can be pushed or not

[Next Scope](scope.md)

---

[Back To Vars](vars.md) //
[Back To Start](start.md)
