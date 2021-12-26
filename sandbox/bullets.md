```load-water-bullet
cycle(1)
sfx(PEW)
if forward == NONE:
  die()
alive:
  walk(RND)
  walk(forward)
  every SECOND:
    die()
  events:
    if event.THUD or event.TOUCH or event.BLOCKED:
      die()
      break
sfx(HIT)
```

### Bullets

Crypto cafe allows you to create custom bullet objects.

[Next Overlays](overlays.md)

---

[Back To Players](players.md) //
[Back To Start](start.md)

