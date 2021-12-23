```load-pushable
cycle(2 * SECOND)

alive:
  follow(find('barrel') ?> nearest())
```

### Scope

Scope is a quick way to find and modify game elements on a board.
There are different categories for these commands query, and filter.

#### Query

 - `find('name')` return a list coords of elements with the given name.
 - `raycast(from, to)` returns a ray a list of coords, and hit coord if the ray hit something.
 - `emptySpace()` returns a list of coords where you can place an object. 
 - `coordsFromRect(x1, y1, x2, y2)` returns a list of coords from the given rectangle. 

#### Filter

##### Detail Filters
These set of filters work both for terrain and objects.

- `with` things

##### Stat Filters
These set of filters work both for terrain and objects.

 - `withLight` if element at coord has this light stat
 - `withCollision` if element at coord has this collision stat
 - `withPushable` if element at coord has this pushable stat

##### Value Filters
These set of filters work only for objects.

- `withValue` if object

##### Distance and Direction Filters
These set of filters work both for terrain and objects.

- `with` things


[Next Overlays](overlays.md)

---

[Back To Details](details.md) //
[Back To Start](start.md)
