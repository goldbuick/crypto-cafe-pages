```load-water-player
cycle(1)
idle()

setLight(MEDIUM)
addDecal('h1', 3, RED, 1, -1)
addDecal('h2', 3, RED, -1, -1)

alive:
  every SECOND:
    walk(RND)
```

### Decals

Decals allow you to place extra non-colliding sprite on your object.

 - `addDecal(name, tile, color, x, y)` adds a new deco sprite to the object
 - `setDecalTile(name, tile)` adds a new deco sprite to the object
 - `setDecalColor(name, color)` adds a new deco sprite to the object
 - `setDecalOrder(name, order)` adds a new deco sprite to the object
 - `setDecalScale(name, scale)` adds a new deco sprite to the object
 - `setDecalCoord(name, x, y)` adds a new deco sprite to the object

[Next Scope](scope.md)

---

[Back To Deco](deco.md) //
[Back To Start](start.md)
