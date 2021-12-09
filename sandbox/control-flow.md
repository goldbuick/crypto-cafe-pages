```load-basic
alive:
  if False:
    talk('hello')
  elif False:
    pass
  else:
    pass

  while False:
    pass

  for i in range(1, 3):
    pass

  every 100:
    talk('100')

  repeat 3:
    pass
    
  events:
    pass
```

### Control Flow

##### If Statements
When the given condition is met, executes the indented block below it

```
if False:
  talk('hello')
```

Also in skripto you use **elif** for an else if statement

##### While Statements
While the condition is met, executes the indented block below it

```
while False:
  pass
```

##### For Statements
Loop over the given array, while setting the given variable to the current value.

```
for v in range(1, 3):
  pass
```

In this example, v will equal 1, 2, then 3 as it loops.

##### Alive Statement
This is a while loop what loops as long as the object is alive.

```
alive:
  walk(RND)
```

##### Every Statement
This is a conditional that executes the indented block below it, every X number of updates.

```
every 100:
  talk('100')
```

##### Repeat Statement
This is a while loop that loops the given number of times.

```
repeat 3:
  pass
```

##### Events Statement
This is a while loop that loops through any events the object has received.

```
events:
  pass
```

[Next Commands](commands.md)

---

[Back To Program Tick](program-tick.md) //
[Back To Start](start.md)
