# Display a scoreboard within a given range

Add a scoreboard to the sidebar that only displays when a player is within a
 given range.

## Setup

Replace `<name>` with the name of the scoreboard you want to display.
Replace `<color>` with the color of the team you want to display the scoreboard for.
Replace `<team_name>` with the name of the team you want to display the
 scoreboard for.

```shell
/scoreboard objectives add <name> dummy
/scoreboard objectives setdisplay sidebar.team.<color> <name>
```

```shell
/team add <team_name>
/team modify <team_name> color <color>
```

## Command blocks

You will need to create two command blocks. They should be repeating,
 always active, and unconditional.

### First command block

```shell
/team leave @a[team=<team_name>]
```

### Second command block

You can change the distance to whatever you want. The distance is in blocks.

```shell
/team join <team_name> @a[distance=..100]
```
