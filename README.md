# 富士山 · Find Fuji

A mobile web app that uses your phone's compass and GPS to tell you exactly which direction to look to see Mt. Fuji — wherever you are in the world.

Pan your phone left and right until the Fuji marker locks onto the crosshair.

**[Try it →](https://fuji-compass.com)**

---

## How it works

1. Grant location and motion permissions when prompted
2. Hold your phone upright and sweep it left and right
3. The viewfinder tracks your heading in real time
4. When the 富士山 marker centres on the crosshair, you're facing Fuji

The bearing and distance update automatically as your GPS position refines. If GPS is unavailable, you can enter a city name or coordinates manually.

## Features

- Works on iOS (Safari) and Android (Chrome)
- Uses `webkitCompassHeading` on iOS and `deviceorientationabsolute` on Android for accurate true-north heading
- Falls back to manual location entry via OpenStreetMap geocoding
- No server, no dependencies — single HTML file

## Browser support

| Browser | Compass | Notes |
|---|---|---|
| iOS Safari | ✅ | Best accuracy |
| iOS Chrome / DDG | ✅ | Uses webkit heading |
| Android Chrome | ✅ | Uses absolute orientation |
| Firefox | ⚠️ | Relative heading only, may drift |
| Desktop | ❌ | No compass sensor |

## Running locally

Just open `index.html` in a browser — no build step needed.

> **Note:** Chrome and Firefox block GPS for `file://` URLs. Use a local server (e.g. `npx serve .`) or deploy to HTTPS for full functionality.

## License

MIT

---

☕ [Buy me a coffee](https://buymeacoffee.com/thuypham)
