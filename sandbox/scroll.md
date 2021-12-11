```load-pushable
cycle(1)
alive:
  every 10 * SECONDS:
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

Here is some content!

[Next Vars](vars.md)

---

[Back To Counters](counters.md) //
[Back To Start](start.md)
