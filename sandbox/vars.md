```load-basic
toggle = 1

alive:
  every 10:
    if toggle:
      walk(RND)
    else:
      shoot(RND)
    toggle = 1 - toggle
```

### Vars

In Skripto you can also make local variables. This is useful if you are doing logic that doesn't require external influence.

You create a local variable by assigning a value to a name. `toggle = 1`

[Next Details](details.md)

---

[Back To Scroll](scroll.md) //
[Back To Start](start.md)
