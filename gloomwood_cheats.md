<img src="/assets/cheattitle.png">
<hr>
<p align="center"><i>This guide was last updated on 7/25/2023</i></p>


## Preface

This guide was created during the Fire at the Gates update! Some information may be incorrect or only applicable to earlier versions of the game! We are trying our best to update it when newer features come out!

## The Runtime Console

The Runtime Console is a console that Gloomwood uses to provide you with a set of commands to modify gameplay features, spawn entities, and more. It is an essential tool for anyone looking to mess with their game, or to make custom saves.

## Unknown Commands

There are currently no new commands that their purposes
are unknown, but some are currently undocumented.

## Obtaining a list of all commands

The `help` command lists every command.

```
help
```

## Enabling Cheats

Enabling cheats allows you to use the `infinite` command.

```
cheats 1
```

As of now, this is the only known use of the `cheats` command.

With this command, do note that `1` and `0` are equivalent to true and false respectively. 
This is the same case for all other commands. 
You cannot use `true` and `false` as arguments.

## Lists

The `list` command lists all registered objects of certain types.
This can work with many types of objects, such as props, weapons,
enemies, and more.

If we wanted to see a list of all `item`s in the game, we could run this command:
```
list items
```
And it would output every item to the Runtime Console.

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

This is where things get interesting.

Spawning entities is done with the `spawn` command.

For an example, let's spawn 20 fishdogs.

To spawn a `fishdog`, type and run this command:

```
spawn ai_fishdog
```

However, one fishdog is boring... why not have 20? Well, to spawn 20 fishdogs, type and run this command:

```
spawn ai_fishdog 20
```

Now, following that logic, if we wanted to spawn an armored huntsman with a rifle, we would run the following:

```
spawn ai_huntsman_armored_rifle
```

All AIs/enemies are prefixed by `ai_`. This is mandatory.

## Spawning Items 

*Note: Spawning items is different from giving yourself items. The `give` command places items directly in your inventory, while the spawn command actually spawns in the item as a physics object (entity)*

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

However, you can still use it to get coordinates of an area easily.

To run it, you would use the following syntax:

```
place marker
```

This would place a `RuntimeMarker` entity at the players position.

## General cheating

There are some commands that allow you to easily modify the way the game/your player behaves. Below are some examples of the commands:

The god command makes your player invulnerable to all damage. If we wanted to turn on godmode, we would run the following:

```
god
```

The thief command will remove all footstep noises and allows you to unlock doors without the key. If we wanted to turn thief mode on, we would run the following:

```
thief 1
```

Or alternatively, just running the command with no arguments will toggle it on/off.

## Giving yourself items and weapons

Giving yourself items is similar to spawning items. The only difference is that items are placed in your inventory, instead of becoming physics objects.

Let's say we want to give ourselves 24 red gem brooches. The command to run would be:

```
give item_brooch_1 24
```

Giving yourself coins is also quite easy. Want to give yourself the max amount of coins (9999)? Want to buy out the Merchant's shop? Run this command:

```
give item_coin 9999
```

*Note: Items that do not fit in your inventory, or do not go in your inventory will be spawned directly on top of you. This includes coins.*

## Disabling and reenabling HUD elements

Managing HUD elementsis done with the `hud` command.

To disable/reenable the entire hud, use the `none` flag:
```
hud none 0
hud none 1
```

*Note: `0` disables the hud element, `1` enables the hud elements.*

To disable/reenable your cursor, use the `cursor` flag:

```
hud cursor 1
```

To disable/reenable your crosshair, use the `crosshair` flag:

```
hud crosshair 0
```

To disable/reenable the unused stealth meter, use the `visibility` flag:

```
hud visibility 1
```

## Saving and loading files

Saving files is done with the `savegame` command. To save to slot 4, run this command:

```
savegame 4
```

Loading files is done with the `loadgame` command. To load slot 4, run this command:

```
loadgame 4
```

You can save and load files outside of the 0-9 range.

```
savegame 100
loadgame -20
```

You cannot save games with strings (text) as the save ID.

## Miscellaneous commands

This section is for commands that don't fit into the other categories.

*TODO*



