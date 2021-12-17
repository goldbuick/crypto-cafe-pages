```load-basic

```

### Scope

Here is some content!

`find('player') ?> withCollision(WALK) ?> withValueGreaterThan(HEALTH, 10)`

Gets re-written as

`withValueGreaterThan(HEALTH, 10, withCollision(WALK, find('player')))`

[Next Overlays](overlays.md)

---

[Back To Details](details.md) //
[Back To Start](start.md)
