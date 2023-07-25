# The Gloomwood "Comprehensive" Guide To Cheating

*This guide was last updated on 7/24/2023*

## Preface

This guide was created during the Fire at the Gates update! Some information may be incorrect or only applicable to earlier versions of the game! We are trying our best to update it when newer features come out!

## The Runtime Console

The `RuntimeConsole` is a console that `Gloomwood` uses to provide you with a set of commands to modify gameplay features, spawn entites, and more. It is an essential tool for anyone looking to mess with their game, or to make custom saves.

## Unknown Commands

There are currently no new commands that their purposes
are unknown, but some are currently undocumented.

## Getting a list of all commands

The `help` command lists every command.

```
help
```

## Enabling Cheats

Enabling cheats allows you to use the `infinite` command.
Just like other `true/false` arguments for some of the other
`RuntimeConsole` commands, `1` is `true` and `0` is `false`.
```
cheats 1
```

As of now, this is the only known use of the `cheats` command.

With this command, do note that `0` and `1` are equivalent to
`false` and `true` respectively. This is true for all commands.

## Lists

The `list` command lists all registered objects of certain types.
This can work with many types of objects, such as `props`, `weapons`,
`entities`, and more.

If we wanted to see a list of all `items` in the game, we could run this command:
```
list items
```
And it would output every item to the `Runtime Console`.

Here is every valid list command:
```
list ai
list corpse
list item
list weapon
list pickup
list prop
list readable
```

## Spawning AIs/Enemies

This is where it gets interesting.

Spawning entities is done with the `spawn` command.

For an example, let's spawn 20 fishdogs.

To spawn a `fishdog`, type and run this command:

```
spawn ai_fishdog
```

However, `one` fishdog is boring.. why not have 20? Well, to spawn `20 fishdogs`, type and run this command:

```
spawn ai_fishdog 20
```

Now, following that logic, if we wanted to spawn an `armored huntsman` with a `rifle`, we would run the following:
```
spawn ai_huntsman_armored_rifle
```

All AIs/enemies are prefixed by `ai_`. This is mandatory.

## Spawning Items 

*Note: Spawning items is different from giving yourself items. The give command places items directly in your inventory, while the spawn command actually spawns in the item as a physics object (entity)*

Spawning items is also done with the `spawn` command.

Let's spawn enough vitalizing tonics for the rest of your life.

```
spawn item_medhypo 50
```

All items are prefixed by `item_`. This is also mandatory.

## Infinite Resources

*Note: As of now, the infinite command only works with ammo.*

The `infinite` command allows you to give yourself an unlimited amount
of any resource. This works by toggling on/off the selected resource type.

If we wanted to give ourselves infinite ammo, we would run this command:

```
infinite ammo 1
```

## Placing Markers
*Note: At the time of writing this, `marker` is the only use input you can provide to the `place` command.*

However, you can still use it to get coordinates
of an area easily.

To run it, you would use the following syntax:

```
place marker
```

This would place a `RuntimeMarker` entity at the players position.

## Altering game mechanics

There are some commands that allow you to easily modify the way the game/your player behaves. Below are some examples of the commands:

The god command makes your player invulnerable to all damage. If we wanted to turn on godmode, we would run the following:

```
god
```

The thief command will remove all footstep noises and remove having to have a key to unlock doors. If we wanted to turn `Thief Mode` on, we would run the following:

```
thief 1
```
Or alternatively, just running the command with no arguments will toggle it `on/off`.

## Giving yourself items and weapons

*TODO*

## Miscellaneous cheats

*TODO*



