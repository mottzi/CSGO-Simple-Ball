# Simple Ball

This is a simple plugin that let's players spawn a ball, pick it up, and kick it (using E). The ball will bounce off of solid structures semi-realistically. 

## Demo

https://github.com/user-attachments/assets/c3bb8219-7ec0-41bb-9610-e8b6715c6641

## Compatibility

This is a [SourceMod](https://www.sourcemod.net/about.php) plugin, so it should be compatible with any game that uses the Half-Life-2 engine (source engine). 

CS 2 is not currently supported, as SourceMod is not yet ported to the source 2 engine.

## Commands

**!ball**: Admin-Menu to set/refresh/remove the ball

## Customization

You can customize the ball by changing the ```#define``` statements at the top of the [source file](addons/sourcemod/scripting/sm_ball.sp). If you do this, keep in mind that you will have to re-compile the plugin before installation.

```c
#define BALL_ENTITY_NAME "simpleball"
#define BALL_CFG_FILE "configs/ballspawns.cfg"
#define BALL_PLAYER_DISTANCE 55.0
#define BALL_KICK_DISTANCE 55.0
#define BALL_KICK_POWER 600.0
#define BALL_HOLD_HEIGHT 15
#define BALL_KICK_HEIGHT_ADDITION 25
#define BALL_RADIUS 16.0
#define BALL_AUTO_RESPAWN 35.0
#define BALL_ADMIN_MENU_FLAG ADMFLAG_BAN
```
