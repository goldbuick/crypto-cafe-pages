```load-pushable
cycle(2 * SECOND)

alive:
  follow(find('barrel') ?> nearest())
```

### Scope

Scope is a quick way to find and modify game elements on a board.
There are different categories for these commands query, and filter.

#### Query

 - `find` things
 - `raycast` things
 - `emptySpace` things
 - `coordsFromRect` things

#### Filter

##### Detail Filters

- `with` things

##### Stat Filters

 - `withLight` if element at coord has this light stat

##### Value Filters

- `with` things

##### Distance and Direction Filters

- `with` things


[Next Overlays](overlays.md)

---

[Back To Details](details.md) //
[Back To Start](start.md)
