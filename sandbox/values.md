```load-basic
set('ammo', 10)
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

* `get('ammo') get a stored value.`
* `set('ammo', 10) set a stored value.`
* `give(10, 'ammo') add 10 to the stored value.`
* `take(10, 'ammo') subtract 10 from the stored value.`
* `has('ammo') returns true if value has been set.`
* `setIfEmpty('ammo', 10) sets stored value only if it has not been set.`

[Next CHAR values](char-values.md)

---

[Back To Lifecycle](lifecycle.md) //
[Back To Start](start.md)
