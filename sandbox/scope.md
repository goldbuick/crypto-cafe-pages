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

- `withTile(tile)` if element at coord has this tile.
- `withColor(color)` if element at coord has this color.

##### Stat Filters
These set of filters work both for terrain and objects.

 - `withLight` if element at coord has this light stat.
 - `withCollision` if element at coord has this collision stat.
 - `withPushable` if element at coord has this pushable stat.

##### Value Filters
These set of filters work only for objects.

- `withValue` if object at coord has this value set.
- `withNotValue` if object at coord does not have this value set.
- `withValueEqual` if object at coord has this value equal to.
- `withValueLessThan` if object at coord has this value less than.
- `withValueGreaterThan` if object at coord has this value greater than.
- `withValueLessThanEqualTo` if object at coord has this value less than or equal to.
- `withValueGreaterThanEqualTo` if object at coord has this value greater than or equal to.

##### Distance and Direction Filters
These set of filters work both for terrain and objects.

- `nearest()` returns nearest coord to self.
- `farthest()` returns farthest coord to self.
- `lessThan(dist)` returns coords less than given distance to self.
- `greaterThan(dist)` returns coords greater than given distance to self.
- `directionIs(dir)` returns coords in the given direction from self.


[Next Overlays](overlays.md)

---

[Back To Details](details.md) //
[Back To Start](start.md)
