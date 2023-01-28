# Object Activator

![Object Activator](../_images/object-activator.png)

Object Activators are a great way to run a set of events when the Game Object becomes active, or when a player or an enemy enters its collider trigger.

**This Component uses an [ULTRAKILL Event](../components/ultrakill-event)**

## Behaviour
There are two cases that can happen:
- If the Object with this component on it doesn't have any collider, it will run the events when it becomes active.
- If the Object has a collider with a trigger on it, events will only run if a player touches the trigger.

## Fields

### One Time
Can only be activated **one** time. Further trying to reenter its trigger or reactivating the Game Object beyond the first time will yield no new results.

### Disable On Exit
If this field is enabled, Events from the [ULTRAKILL Event](../components/ultrakill-event) are reverted when either:
- The Game Object becomes inactive
- The Player leaves the Trigger

Objects under `To Activate Objects` become inactive, objects under `To Dis Activate Objects` become active, and `On Dis Activate()` events run.

### Dont Activate On Enable
If this is enabled, events will not be activated when the object becomes active.

### Reactivate On Enable
This is required for non-trigger based Object Activators. If you want to run the events every time the Game Object becomes active, this has to be enabled, even if `One Time` is not ticked.

### Delay
Events will ran after specified amount of time in seconds. Can use decimal numbers. This can be cancelled if the Object Activator gets deactivated (example deactivating the Game Object its on,
or leaving the trigger if [`Disable On Exit`](/components/object-activator#disable-on-exit) is enabled.)

### OBAC
Requires a Game Object that has an Object Activation Check component on it. If its status is enabled, the Object Activator will run, otherwise it won't.

The status can be controlled using [ULTRAKILL Events](../components/ultrakill-event)

### Events
See [ULTRAKILL Event](../components/ultrakill-event.md) for further information.

This will be executed based on the conditions descripted in [Behaviour](/components/object-activator#behaviour).

### For Enemies
If the Game Object that has an Object Activator also has a trigger on it, it will only be able to be triggered by enemies.

## Functions
Functions can be called from [ULTRAKILL Events](../components/ultrakill-event).

### Activate()
Triggers the events from [Events](/components/object-activator#events) regardless of conditions, without delay.

### ActivateIfActive()
Triggers the events from [Events](/components/object-activator#events) if conditions are met.

### Deactivate()
Deactivates the Object Activator, and [reverts the events](../components/ultrakill-event.md##on-dis-activate). If [One Time](/components/object-activator#one-time) was enabled, it resets its state so it can be used again.