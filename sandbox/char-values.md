```load-basic-player
cycle(25)

setIfEmpty('test', 1000, CHAR)

alive:
  talk('!' + get('test', CHAR))
  take(1, 'test', CHAR)
  repeat 7:
    idle()
```

### CHAR Values

Char values are special in that they work across different games and play sessions.

Observe what happens when refresh the page.

[Next Built Ins](built-ins.md)

---

[Back To Values](values.md) //
[Back To Start](start.md)
