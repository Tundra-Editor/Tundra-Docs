# Optimization

Bigger maps need some help from you to run smoothly.

## Disabling Rooms

This technique is used in every stock ULTRAKILL map. It works by keeping all rooms disabled and only enabling them when a neighboring door opens.

Level 0-2 in the editor.

![Level 0-2](_images/level-0-2-disabled-rooms.png)

An example door component configured to disable and enable certain rooms.

![Door Component with Activated Rooms](_images/door-with-activated-rooms.png)

The [FirstRoom](setup?id=first-room) prefab configured to enable the first actual room before opening the main door.

![The First Room Prefab Component](_images/first-room-prefab-rooms.png)
