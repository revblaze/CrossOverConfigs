# CrossOverConfigs
Optimal CrossOver configurations for Apple Silicon (with installation)

"My installer won't launch in Crossover."

## Advanced Install (Headless)

1. Install an unlisted application
2. Select installer executable
3. `...` button → Advanced Options
4. `+` button, add the following programs to install:

```
CrossOver HTML engine
Wine Mono
Microsoft Visual C++ 6.0 (4.2 & 6.0) Redistributable
Microsoft Rich Edit 4.1 (Msftedit.dll)
msls31
Microsoft Rich Edit 2.0
```

And potentially: `DirectX for Modern Games`


## Easier Install (Steam Client Overhead)

1. CrossOver.app > Install
2. Select "Steam"
3. In the `CrossOver will install 'Steam' into a new Windows 10 64-bit bottle named 'Steam'` row, click "Edit"
4. In the "New Bottle Name" field, type the name of the game you're attempting to install
5. Follow the on-screen instructions to install Steam; deselect "Open Steam" at the end (or just close it after)
6. Open the newly created Bottle from the CrossOver.app left sidebar menu

<i>\* Steam comes pre-packaged with a number of frameworks and libraries that most installers will assume you already have. This is why we setup a new bottle with Steam.</i>

### Workaround 1: CrossOver + Steam Fix
Try this workaround first.

1. Click "Install Application into Bottle"
2. Select the installer exe that wasn't launching.

If your game still won't launch, continue on. Do not remove the new bottle with Steam, as we'll still need it.

### Workaround 2: Virtual Machine
You'll need a virtual machine running Windows 10 for this next step. VMWare is free for non-commercial users. You can delete the virtual machine after your installation is complete.

1. Run the installer from a virtual machine, preferably running Windows 10
2. Note down where the game is installed to (ie. `C:\Games\My-Game`)
3. Go to your newly created CrossOver bottle (left sidebar) and select "Open C: Drive"
4. This should open Finder; from here, open the folder `Program Files (x86)`
5. Move the game from your virtual machine running Windows to the `Program Files (x86)` folder
  - ie. `C:\Ganes\My-Game` → `Program Files (x86)/My-Game`
  - Most virtual machines support dragging and dropping from Windows file manager into Finder
6. Run the exe game file from the newly moved folder (ie. `Program Files (x86)/My-Game/Game.exe`)



## Package Prerequisites
<i>You may only need the x64 packages with CrossOver.</i>

```
Dragon Age: Inquisition
C++ Redist 2008 SP1 x86
C++ Redist 2008 SP1 x64
C++ Redist 2010 SP1 x86
C++ Redist 2010 SP1 x64
C++ Redist 2012 x86
C++ Redist 2012 x64
C++ Redist 2013 x86
C++ Redist 2013 x64

Dishonered: Complete
C++ Redist 2012 x86
C++ Redist 2012 x64

Sekiro: Shadows Die Twice
C++ Redist 2015 x86
C++ Redist 2015 x64

Batman: Arkham Knight
C++ Redist 2010 SP1 ×86
C++ Redist 2010 SP1 ×64
C++ Redist 2012 x86
C++ Redist 2012 ×64
Microsoft NET Framework 4.5.1

Aliens: Dark Descent
C++ Redist 2015-2019 x86
C++ Redist 2015-2019 x64
```
