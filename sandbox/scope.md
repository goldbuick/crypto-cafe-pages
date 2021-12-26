```load-pushable
cycle(2 * SECOND)

alive:
  follow(find('barrel') ?> nearest())
```

### Scope

Scope is a quick way to find and modify game elements on a board.
There are different categories for these commands: query, and filters.

##### Query

 - `find('name')` return a list coords of elements with the given name.
 - `raycast(from, to)` returns a ray a list of coords, and hit coord if the ray hit something.
 - `emptySpace()` returns a list of coords where you can place an object. 
 - `coordsFromRect(x1, y1, x2, y2)` returns a list of coords from the given rectangle. 

##### Detail Filters
These set of filters work both for terrain and objects.

- `withTile(tile, coords)` if element at coord has this tile.
- `withColor(color, coords)` if element at coord has this color.

##### Stat Filters
These set of filters work both for terrain and objects.

 - `withLight(light, coords)` if element at coord has this light stat.
 - `withCollision(collision, coords)` if element at coord has this collision stat.
 - `withPushable(pushable, coords)` if element at coord has this pushable stat.

##### Value Filters
These set of filters work only for objects.

- `withValue(name, value, coords)` if object at coord has this value set.
- `withNotValue(name, value, coords)` if object at coord does not have this value set.
- `withValueEqual(name, value, coords)` if object at coord has this value equal to.
- `withValueLessThan(name, value, coords)` if object at coord has this value less than.
- `withValueGreaterThan(name, value, coords)` if object at coord has this value greater than.
- `withValueLessThanEqualTo(name, value, coords)` if object at coord has this value less than or equal to.
- `withValueGreaterThanEqualTo(name, value, coords)` if object at coord has this value greater than or equal to.

##### Distance and Direction Filters
These set of filters work both for terrain and objects.

- `nearest(coords)` returns nearest coord to self.
- `farthest(coords)` returns farthest coord to self.
- `lessThan(dist, coords)` returns coords less than given distance to self.
- `greaterThan(dist, coords)` returns coords greater than given distance to self.
- `directionIs(dir, coords)` returns coords in the given direction from self.


[Next Players](players.md)

---

[Back To Decals](decals.md) //
[Back To Start](start.md)
