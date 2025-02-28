# SimpleAutoRestart

[![github](https://cdn.jsdelivr.net/npm/@intergrav/devins-badges@3/assets/cozy/available/github_vector.svg)](https://github.com/teunjojo/SimpleAutoRestart)
[![spigot](https://cdn.jsdelivr.net/npm/@intergrav/devins-badges@3/assets/cozy/supported/spigot_vector.svg)](https://www.spigotmc.org/resources/simpleautorestart.107932/)
[![modrinth](https://cdn.jsdelivr.net/npm/@intergrav/devins-badges@3/assets/cozy/available/modrinth_vector.svg)](https://modrinth.com/plugin/simpleautorestart)
[![curseforge](https://cdn.jsdelivr.net/npm/@intergrav/devins-badges@3/assets/cozy/available/curseforge_vector.svg)](https://www.curseforge.com/minecraft/bukkit-plugins/simpleautorestart)

I tried many of the auto restart plugins out there, but all I could find were either too complex or tick based. This means they were not accurate when TPS drops below 20 and therefore not compatible with plugins like [Hibernate](https://www.spigotmc.org/resources/hibernate.4441/) and [Server Naptime](https://github.com/gvk/MinecraftPluginServerHibernate).

So I decided to create my own.

[![bstats](https://bstats.org/signatures/bukkit/simpleautorestart.svg)](https://www.bstats.org/plugin/bukkit/SimpleAutoRestart/17760)

## Features
- Schedule automatic restarts at a specific times.
- Warning messages broadcasted to players before restart.
- Schedule multiple restarts.
- Realtime based and not tick based for more accurate.
- Compatible with plugins like [Hibernate](https://www.spigotmc.org/resources/hibernate.4441/) and [Server Naptime](https://github.com/gvk/MinecraftPluginServerHibernate)

## What is looks like in game (although you can customize this):
![Chat](https://i.imgur.com/ZjQq3sq.png)

## What is looks like in the server console (although you can customize this):
![Console](https://i.imgur.com/Kshy5U5.png)

## Installation
1. Download `SimpleAutoRestart-x.x.x-jar` from the releases page.
2. Place the JAR file in the plugins folder of your server.
3. Start or restart the server.
4. Configure the plugin by editing the config.yml file in the plugins/SimpleAutoRestart folder.

## Configuration
```
# The hour and minute when the server should restart (24 hour format)
restartTime:
- '00:00'
# Add multiple times by adding a new line like: - '12:00'

# Configure message and the corresponding pre-warning time in seconds
messages:
  '0': 'Restarting now'
  '1': 'Restarting in 1 second'
  '2': 'Restarting in 2 seconds'
  '3': 'Restarting in 3 seconds'
  '60': 'Restarting in 1 minute'
  '120': 'Restarting in 2 minutes'
  '180': 'Restarting in 3 minutes'
  '300': 'Restarting in 5 minutes'

titles: 
  '300' : '§l§4Warning'
  '3' : '§l§4Warning'

subtitles:
  '300' : "§6Restarting in 5 minutes"
  '3' : "§6Restarting now..."
```

## Commands
- `/simpleautorestart` or `/sar` or `/autorestart` - Show the help menu.
- `/simpleautorestart cancel` - Cancel the next restart.
- `/simpleautorestart resume` - Resume the next restart.
- `/simpleautorestart status` - Show the status of the next restart.
- `/simpleautorestart set <hour> <minute>` - Schedule a restart at a specific time.

## Support
If you have any issues or questions. Feel free to [create an issue ticket](https://github.com/teunjojo/SimpleAutoRestart/issues/new). 

