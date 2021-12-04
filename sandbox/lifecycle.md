```load-water
cycle(25)
alive:
  walk(RND)
  walk(RND)
  walk(RND)
  walk(RND)
  walk(RND)
  talk('watch out!')
  idle()
  shoot(RND)
  shoot(RND)
  shoot(RND)
  shoot(RND)
  idle()
  if blocked(UP):
    talk('I am blocked!')
```

### Lifecycle

Lifecycle commands mostly deal with moving, creating, and removing game elements. 

Instead of `talk('I am blocked!')` try changing it to `die()` to see what happens.

[Next Values](values.md)

---

[Back To Commands](commands.md) //
[Back To Start](start.md)
