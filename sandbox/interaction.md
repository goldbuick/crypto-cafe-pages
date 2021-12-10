```load-water
alive:
  walk(RND)
  events:
    if player(event.TOUCH):
      talk('player hit me')
    if bullet(event.TOUCH):
      talk('bullet hit me')
    if player(event.THUD):
      talk('I ran into the player')
    if event.BLOCKED:
      talk(event.BLOCKED)      
```

### Interaction

As objects move and bump into things it causes events.
Objects can also send custom events to each other.
And we use a special loop `events:` to handle events.

[Next Counters](counters.md)

---

[Back To Built-Ins](built-ins.md) //
[Back To Start](start.md)
