```load-basic
cycle(25)
walk(NONE)
talk('setup')

alive:
  walk(NONE)
  walk(NONE)
  walk(NONE)  
  talk('alive')  
  walk(RND)
  walk(RND)
  walk(RND)
  die()

talk('dead')
walk(NONE)
```

### Program Flow
Skripto has 3 basic parts to it.

##### setup
the code that runs before the alive: loop

##### alive
the code that repeats while the object is alive

##### dead
the code that runs after the alive: loop, but before the object is destroyed

---

[Next Program Tick](!SANDBOX_PROGRAM_TICK)

---

[Back To Start](!SANDBOX_START)
