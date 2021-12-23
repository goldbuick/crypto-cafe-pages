```load-water-player
cycle(1)
set('HEALTH', 100)
give(1, [RED,'KEY'])

counterNumber('HEALTH', 'Health')
counterItem([RED,'KEY'], 'KEY', 12, RED)

alive:
  if input.MOVE:
    walk(input.DIR)
  events:
    if bullet(event.TOUCH):
      sfx(EXPLODE)
      take(1, 'HEALTH')
```

### Counters

Counters are a quick way to display player object values to the person playing your game.

[Next Scroll](scroll.md)

---

[Back To Interaction](interaction.md) //
[Back To Start](start.md)
