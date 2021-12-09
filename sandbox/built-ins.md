```load-darkness
cycle(25)
setLight(SMALL)

alive:
  die()
  
sfx(EXPLODE)
```

### Built-Ins

Skripto has built-in constants for common things.

##### dir
  * `NONE` no direction.
  * `UP`
  * `DOWN`
  * `LEFT`
  * `RIGHT`
  * `RND` pick a random direction. 

##### light
  * `OFF` light radius of 0.
  * `SMALL` light radius of 3.
  * `MEDIUM` light radius of 5.
  * `LARGE` light radius of 10.

##### collision
  * `SOLID` cannot be walked through, or swam through.
  * `WALK` can walk on walkable terrain, will be blocked by swimmable terrain.
  * `SWIM` can swim on swimmable terrain, will be blocked by walkable terrain.
  * `BULLET` can move through both walkable and swimmable terrain.
  * `GHOST ` can move through any kind of terrain.

##### colors
  * `link to colors page in docs goes here ... `

##### values
These are some common names for use with get() & set(). ie: get(HEALTH), etc...
  * `HEALTH`
  * `AMMO`
  * `GEMS`
  * `TORCHES`
  * `SCORE`
  * `KEY`

##### sound
These are names for the built-in sound effects.
  * `CHOOSE`
  * `COIN`
  * `EXPLODE`
  * `HIT`
  * `JUMP`
  * `POWERUP`
  * `PEW `

##### math
  * `PI` value of pi.
  * `SECOND` value of 25, since there are 25 ticks per second.

##### globals
  * `SELF` target current object.
  * `BOARD` get/set from board values.
  * `GAME` get/set from game values.
  * `CHAR ` get/set from char values.

[Next Interaction](interaction.md)

---

[Back To Char Values](char-values.md) //
[Back To Start](start.md)
