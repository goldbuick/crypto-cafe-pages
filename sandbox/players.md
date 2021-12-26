```load-basic-player
cycle(1)
set('health', 100)
counterNumber('health', 'health')

alive:
  if input.MOVE:
    walk(input.DIR)
  if input.SHOOT:
    shoot(input.DIR)
  if input.ACTION_1:
    teleport(select('basic', 'water', 'pushable'))

  events:
    if bullet(event.TOUCH):
      take(1, 'health')
```

### Players

Crypto cafe allows you to create custom player objects.


[Next Bullets](bullets.md)

---

[Back To Scope](scope.md) //
[Back To Start](start.md)

