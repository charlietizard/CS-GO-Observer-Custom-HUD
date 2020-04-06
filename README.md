# NSE CS:GO Observer Custom HUD
Shout-out to:
[RedSparr0w](https://github.com/RedSparr0w)
and
[osztenkurden](https://github.com/osztenkurden)
for base code!

## How does it work?
Basically, CS:GO is streaming data to local app-server, that transformes data and then load it to local webpage.

## To-do before running
- Node.js needs to be installed
- public/files/cfg/gamestate_integration_observerspectator.cfg needs to be placed in cfg folder in CS:GO location
- public/files/cfg/observer.cfg needs to be placed in cfg folder in CS:GO location
- CS:GO needs to run on Fullscreen Windowed (I know people may dislike it, but since it's only for observation, soo...)
- After running CS:GO and connecting to match (or replaying a demo, you can use this in  it too), type to console `exec observer.cfg`, it makes everything default disappear besides map and killfeed 

## Configuration
```javascript
//config.json
{
    "GameStateIntegrationPort":1337, //This must be the same as in gamestate_integration_observerspectator.cfg,
    "ServerPort":2626, //Some free port on your PC
    "SteamApiKey":"ABCDEFGIJK12345678", //Steam API Key, without it avatars won't work
    "DisplayAvatars":true, // true for yes, false for no
    "AvatarDirectory":"./public/files/avatars/", // Local storage for avatars
    "GSIToken":"120987" //This must be the same as in gamestate_integration_observerspectator.cfg
}
```

## Examples
Coming soon

## Setting up video
Check [osztenkurden's project](https://github.com/osztenkurden/CS-GO-Observer-Custom-HUD) for this info.

