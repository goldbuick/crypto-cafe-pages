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

[Next Details](details.md)

---

[Back To Scroll](scroll.md) //
[Back To Start](start.md)
