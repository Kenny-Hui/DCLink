# DCLink

## Why
I can't find a decent Discord Chat Linking Bot that suits my need and runs on Fabric 1.17.1

[Chatter](https://github.com/axieum/chatter) is what I used to use, but it's on 1.16.5.
While a newer rewritten mod, [Minecord](https://github.com/axieum/minecord) is only available for 1.19.

Unfortunately I don't have enough understanding of the code to port either of the mod to 1.17, so I made my own mod (Where I'll probably forget the code in about a year or so)

What a great idea!

## Features
- Fabric 1.16.5 - 1.19.1
- Can reload config
- Support bot activities
- Support showing replied message from Discord to MC
- Automatically fetch custom guild emoji, show properly when relaying to Discord
- Dynamically toggle outbound/inbound messages

### Supported Server Events to be relayed to Discord
- Server Starting / Started / Stopping / Stopped
- Server Crash

### Supported Player Events to be relayed to Discord
- Player Join
- Player Leave
- Player send chat message (Including commands)
- Player entering another dimension
- Player Death (WIP)

## Future Goals
- Player Advancement Events
- Relay Discord Reaction Event to Minecraft
- Add Discord Commands
- Allow exporting config to other Discord relaying mod
- Touch some grass

## Downloads
**This is not production ready yet, only use if you know what you are doing!**

For downloading the latest build, please [click here](https://github.com/Kenny-Hui/DCLink/actions).

However no support will be provided, nor any guarantee on compatibilities, given that this is still a very early WIP

## Cross Version Mapping
For easier development, all version-specific code is stored in `src/main/mappings`.

The files will then be copied over to `src/main/java/com/lx/dclink`.

To change the Minecraft version, edit the **default_minecraft_version** in `build.gradle`.
(Or if you simply want to build, `./gradlew build -PbuildVersion=<Minecraft Version Here>`)

## License
This project is licensed under [MIT License](https://opensource.org/licenses/MIT)