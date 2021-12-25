```load-water-player
cycle(1)

alive:
  if input.WALK;
    walk(input.DIR)
  if input.SHOOT:
    shake()
    talk('no ammo!')
  if input.ACTION_1:
    spin(0)
  if input.ACTION_2:
    spin(2)
  if input.ACTION_3:
    spin(8)
  if input.ACTION_4:
    spin(16)
  events:
    if event.THUD or event.BLOCKED:
      bump()
```

### Deco

These commands are helpful with animation and displaying temporary text over an object.

##### Talk
 - `talk(msg)` displays a text message above and object for a short period of time

##### Animation
 - `bump()` makes the object animate like it has bumped into something
 - `shake()` makes the object animate like it is shaking
 - `spin(rate)` makes the object spin continuously at the given rate, spin(0) will stop the spin

[Next Decals](decals.md)

---

[Back To Details](details.md) //
[Back To Start](start.md)
