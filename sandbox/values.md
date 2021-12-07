```load-basic

```

### Values

Values are a way of storing data in objects, in boards, in your game, and in a character file.

##### Setting Values

```
set('ammo', 10)
```

This will set **ammo** to **10** on the object

With all the value related commands you pick which source of data to use.
* Don't include a target or **SELF** and the data comes from the object
* Target is **BOARD**, this get/sets from board values. This means any object on the board can access these values.
* When target is **GAME**, this get/sets from game values. This means any object on any board can access these values. 

##### Value Commands

* `get('ammo')`
* `set('ammo', 10)`
* `give(10, 'ammo')`
* `take(10, 'ammo')`
* `has('ammo')`
* `setIfEmpty('ammo', 10)`

[Next CHAR values](char-values.md)

---

[Back To Lifecycle](lifecycle.md) //
[Back To Start](start.md)
