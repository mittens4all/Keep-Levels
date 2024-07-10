
# Keep Levels

This behavior pack uses scoreboards to detect player experience levels. Experience levels are not lost after dying and remain upon respawn.

## Installing the pack:

Add the Keep Levels Add-on to your behavior packs on your world. Behavior packs disable achievements, but editing the world with an NBT editor can re-enable achievements when uploading your world to a realm.

Re-enable achievements on either pc or mobile with the free NBT editor [Dovetail](https://github.com/Offroaders123/Dovetail) 

### How to use the scoreboard

The pack is ready to work after adding to your world. If a player dies, they keep their levels, just like with `/gamerule keepinventory true` but still lose their inventory.

You can display a player's levels by setting the scoreboard display.

```js
/scoreboard objectives setdisplay sidebar xp_level
```

Removing levels from a player, like in an NPC Shop or using abilities, will make the score go down. However, removing scores from **`xp_level`** will not remove experience levels.

```js
/xp -10L @p` \\ Scoreboard objective xp_level goes down.
```

It works functionally the same as the target selectors **`l`** and **`lm`**. The examples below do the same thing.

```js
/execute as @a[lm=10, l=15] run effect @s strength 0 1 true
```
```js
/execute as @a[scores={xp_level=10..15}] run effect @s strength 0 1 true
```

## Authors

- [@mittens4all](https://www.github.com/mittens4all)
- [Youtube](https://www.youtube.com/@mittens4all)

```js
       _                              _     _       _ _  
      (_)  _     _                   | |   (_)     | | | 
 ____  _ _| |_ _| |_ _____ ____   ___| |_____ _____| | | 
|    \| (_   _|_   _) ___ |  _ \ /___)_____  (____ | | | 
| | | | | | |_  | |_| ____| | | |___ |     | / ___ | | | 
|_|_|_|_|  \__)  \__)_____)_| |_(___/      |_\_____|\_)_)
                                                         
```
