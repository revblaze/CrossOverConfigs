# CrossOverConfigs
Optimal game installations and configurations for CrossOver (no Steam).

<i>"My installer won't launch in Crossover"</i> or <i>"I already have the installed game files, I just want to run them through CrossOver."</i>

## Manual Install of New Game (Headless)

1. Open CrossOver.app, `Bottle > New Bottle...`
2. New Bottle Name: `[Name of Game]`
3. Select Windows version (`Windows 10 64bit` if unsure)
4. Click **Create**
5. Select new bottle from left-hand panel, click "Install Application into Bottle" from right-hand panel
6. In the search bar, type `C++ 6.0` and select the package with title `Microsoft Visual C++ 6.0 (4.2 & 6.0) Redistributable`
7. Click the top-right button of the cirlce with 3 dots, select `Advanced Options...`
8. See each page for notes on package dependencies and which to install (if unsure, select `Visual C++ 2015-2022 (64-bit)`
9. Click `Done`, then `Install` and walkthrough the installation windows
10. Follow the instructions for Installation Type A or Type B below...

### A) Installation Setup
<i>Follow this step for running game installers. If you already have the full game files (ie. pre-installed via Parallels/VMware), go to `Step B)`.</i>
1. Return to new bottle from left-hand panel, click "Install Application into Bottle" from right-hand panel
2. Select the top-right button "Install an unlisted application"
3. Click the "Install" button and locate your game installer exe file
4. Follow through with the installation process
5. Double-click the icon of your new game icon to start playing

<i>If the game installer will not launch with CrossOver, you will likely need to install these game files through a virtual machine (Windows running on Parallels/VMware). Then copy the files from that installation to your Mac and perform `Step B)`.</i>

### B) Pre-Installed Setup
<i>Follow this step if you already have the full game files pre-installed and ready to go (ie. Parallels/VMware).</i>
1. Return to new bottle from left-hand panel, click "Open C:Drive" from right-hand panel
2. Copy the pre-installed game folder/directory into this folder/directory
3. Return to CrossOver.app and select "Run Command"
4. Click `Browse...` and select the game-launching exe file from the copied folder/directory
5. Click `Save Command as a Launcher` and wait (do not close this window)
6. Once an icon of your game shows up in the CrossOver window (behind this window), you may close this window
7. Double-click the icon of your new game icon to start playing


## Package Prerequisites
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
