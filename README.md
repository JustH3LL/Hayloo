**I decided to put together a copy of Halo CE with much-needed quality-of-life improvements. This copy will *not* work at schools, unfornately. This is specifically for those at home.**
----------------------------------------------

__The improvements are as follows:__

-    **1.10 patch**    https://halo-fixes.forumotion.com/t6-manual-1-10-update-for-players-with-unofficial-copies
    -    This is pretty much manditory if you want to play online. Gamespy is dead, kiddo.
    
-    **Halo AntiCheat 2 (HAC2)**    http://198.98.120.174/index.html
    -    I included this to have the functionality of downloading maps in-game when you attempt to join a server
    
-    **Chimera**    https://opencarnage.net/index.php?/topic/6916-chimera-build-49/
    -    Those sweet interpolated animations and other visual improvements, including FOV. You *could* use HAC to change FOV as well, but I recommend using this instead. HAC doesn't like remembering your FOV setting and tends to forget it.
    
-    **Halo CE Refined campaign maps**    https://haloce3.com/downloads/singleplayer/modified-singleplayer/refined-halo-1-singleplayer-maps/?_sft_category=modified-singleplayer
    -    The campaign but with less broken visuals and a nice HD remake of the UI (note that the UI will only be present in the Combat Evolved campaign due to how the Halo CE engine functions.)
    
-    **Universal UI**    http://hce.halomaps.org/index.cfm?fid=6952
    -    A way better main menu.
    

----------------------------------------------

**Now that's out of the way, you can download it here:**

__**Halo Custom "Unfucked" Edition:**__ https://drive.google.com/open?id=1-rvR5Fk59YNmyEBU4pnwb3bT5j0VXzeh


**BUT FIRST**

You *have* to run a few commands to set it up properly. Firstly, any sort of chat functionality is 99% likely to be broken out of the box. There is a fix, but there also is an issue with the game being so fucking old that it will have a persistent error box in the top left if you touch 1080p if you use said fix. Secondly, when you download the game, you will notice a batch file called `haloce.bat`. Open it in notepad.

it should look like:

```START haloce.exe -console -vidmode 1366,768,60```

There are two launch flags here, the first launches Halo CE with the capability to open the game console, which we will need. Right now, we will focus on the vidmode flag. This flag tells Halo to launch at the specified resolution and refresh rate, using three parameters. The first parameter is your horizontal resolution, the second is vertical resolution, and final parameter is your refresh rate. If you don't know what your refresh rate is, just keep it at 60. Edit these parameters to your monitor's resolution, and then once you're done, save the file. 

Once it is saved, close notepad as you will no longer be needing it. Launch the haloce.**bat**

Pull up the command prompt with the ~ key, and type these commands:

`chimera_interpolate 9`
`chimera_uncap_cinematic 1`
`chimera_block_lod 1`
`chimera_block_zoom_blur 1`
`chimera_af 1`
`redirect_kill_feed 1`
`custom_chat 1`

and then there's:

`chimera_vertical_fov`

Set this to your liking. Personally, I go with 90 on most things. That's all there is to make it not shit, just remember to launch with the batch file if you want to keep your resolution. Or maybe my system is just retarded and won't show other resolution options like it should, who knows.

You'll notice a whole bunch of other stuff in the campaign menus and firefight menus (yes, firefight). Universal UI included a nice little PDF with the links to literally everything, which can be access here for your convenience.
