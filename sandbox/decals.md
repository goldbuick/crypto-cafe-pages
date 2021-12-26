```load-darkness
cycle(1)
idle()
 
setTile(5)
setColor(ORANGE)
setLight(MEDIUM)

addDecal('h1', 3, RED, 1, -1)
setDecalOrder('h1', 1)
setDecalScale('h1', 2)

addDecal('h2', 3, RED, -0.5, -1)
setDecalOrder('h2', 3)
setDecalScale('h2', 0.5)

addDecal('h3', 3, RED, 0, -1)
setDecalOrder('h3', 2)

alive:
  find('bullet') ?> setLight(SMALL)
  every SECOND:
    walk(RND)
```

### Decals

Decals allow you to place extra non-colliding sprite on your object.

 - `addDecal(name, tile, color, x, y)` adds a new deco sprite to the object
 - `setDecalTile(name, tile)` updates tile on a deco sprite
 - `setDecalColor(name, color)` updates color on a deco sprite
 - `setDecalOrder(name, order)` updates draw order on a deco sprite
 - `setDecalScale(name, scale)` updates scale on a deco sprite
 - `setDecalCoord(name, x, y)` updates draw coords on a deco sprite

[Next Scope](scope.md)

---

[Back To Deco](deco.md) //
[Back To Start](start.md)
