µBMSC
=====
µBMSC is a modified version of iBMSC to add features and clean up the iBMSC code, fix bugs and so on.
See README.md.old for original iBMSC README file.

**BMSdori**
=====
* TODO:
  * Set note color based on known Bandori note labels
      * PROGRESS: 
          * Added code to change color of notes. Works for regular notes, flicks, sliderends, and skill notes
          * Wanted to mark "dangling" slider notes red. Not working properly right now as all slide notes are being colored red.
  * Render lines between slide notes for easier visualization
      * PROGRESS:
          * Logic behind it looks good, but I need to learn how to draw stuff that isn't a rectangle lol
          * Still need to figure out how to split a single note LN into head, body, and tail
          * Coloring skill activation LNs is gonna be kinda fucky but I think I can make it work.
  * Create blank file with WAV labels preset for Bandori charts
  * Keyboard shortcuts to change between Bandori note types
  
* I don't even know how to use the BMS previewers myself, so I'll figure that out later. Would be cool to create a custom previewer using Burrito's code for bandorichart.

Changes
=====
* Out of the box OGG previews
  * Seeks for WAV if OGG doesn't exist, and viceversa
* Bugfixes
  * BMSE clipboard input fixed
* Additions
  * Landmine support (Shift + Ctrl + Click)
  * Several new encodings (EUC-KR, Shift-JIS)
  * Go To Measure (Ctrl+G)
  * Mouse Row/Column Highlight
  * Ctrl+Scroll wheel changes zoom level
  * Huge BPM support (10e12)
  * UI improvements
  * **Time select mode** Convert Area to Stop 
  * **Select Mode** Select notes with labels on screen, all notes with labels (Shift+Ctrl+Click, Shift+Ctrl+A)
  * Non-locale dependant number output (No more commas instead of periods)
  * **Write mode** Autowav Increase functionality 
  * **dtinth** Move and Deselect (Shift+Number)
  * **NS-Kazuki** #SCROLL Support
* Development
  * Codebase reorganized for developers


Check appveyor for automated builds.
[![Build status](https://ci.appveyor.com/api/projects/status/m7iygj9sje2yqf43?svg=true)](https://ci.appveyor.com/project/zardoru/ibmsc)
