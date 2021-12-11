```load-pushable
cycle(1)
alive:
  every 10 * SECOND:
    talk('bump into me')
    
  events:
    if player(event.TOUCH):
      scroll('Hey Thanks!', event.TOUCH)
      text('Here is a basic scroll with some options')
      pick(1, 'One')
      pick(2, 'Two')
      pick(3, 'Three')
      
    if event.SCROLL:
      scroll('You picked ' + event.PICK)
```

### Scroll

Scrolls are a quick way to show the player messages as well as give them options to pick.

```
scroll('Thing', event.TOUCH) # Send scroll to one player referenced by event.TOUCH.
scroll('Thing') # Send the scroll to any player on the board.
```

[Next Vars](vars.md)

---

[Back To Counters](counters.md) //
[Back To Start](start.md)
