---
title: Game State
---

You can access information on the current state of the game.

## Mode
Your robot can be in 2 modes, `DEVELOPMENT` and `COMPETITION`. During competition mode, your robot will stop executing at the end of the match.

```python
from robot.game import GameMode

r.zone == GameMode.DEVELOPMENT
>> True
```

## Zone
The corner your robot starts in, known as its _zone_, is stored in the zone property. This is `0` by default.

```python
r.zone
>> 0
```
