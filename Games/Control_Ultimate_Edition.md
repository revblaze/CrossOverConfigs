# Control Ultimate Edition

## CrossOver Config
- [x] D3DMetal
- [x] Esync
- [x] High Resolution Mode

## Custom Setup
1. `Open C: Drive` for bottle
2. Note the directory path
3. Back to CrossOver, `Run Command`
4. Command: click `Browse...`
6. Select the DirectX 12 launcher
7. Click the `"Save Command as a Launcher"` button
8. Launch to render resolution config, exit out
9. Download and install the [HDR ULTRAWIDE PATCH](https://www.nexusmods.com/control/mods/90)
10. Open `renderer.ini`, modify the following config:

```
"m_iOutputResolutionX": 3456,
"m_iOutputResolutionY": 2234,
"m_iRenderResolutionX": 2560,
"m_iRenderResolutionY": 1600,

...

"m_bSkipIntroVideos": true
```
