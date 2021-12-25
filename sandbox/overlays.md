```load-basic
cycle(1)
idle()

alive:
  every 2 * SECOND:
    walk(RND)
  
  events:
    if player(event.TOUCH):
      set('open', event.TOUCH)

  if has('open'):
    openOverlay('overlay', get('open'))
    clear('open')
```

### Overlays

Overlays are a way to have custom UI in your game. When a board is run as an overlay, all objects on the board get input from the player.

Here is the code to object on the example sandbox overlay.

```
cycle(1)
alive:
  events:
    if event.THUD:
      sfx(HIT)
      bump()
    if input.MOVE:
      walk(input.DIR)
    if input.SHOOT:
      talk('PEW PEW!')
    if input.ACTION_1:
      sfx(COIN)
    if input.ACTION_2:
      closeOverlay()
    if input.ACTION_3:
      sfx(EXPLODE)
    if input.ACTION_4:
      play('https://www.beepbox.co/#9n31s0k0l.....')
```

---

[Back To Scope](scope.md) //
[Back To Start](start.md)
