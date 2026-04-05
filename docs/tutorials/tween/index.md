---
title: Tweening
description: Examples on how to use Tweens
---

**!! WORK IN PROGRESS !!**

Basic Tween
```lua
local part: Part = script.Parent
local origin = part.Position
local tw = Tween:NewTween()

print("Tween Start!")

tw:TweenVector3(origin, origin + Vector3.New(0, 10, 0), 10, function(val)
    part.Position = val
end)

tw.Finished:Wait()

print("Tween Finished!")
```