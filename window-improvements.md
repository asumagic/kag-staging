# Window and input improvements

Windowing is now done using SDL2 rather than Irrlicht, which should be more reliable.  
This resulted in an additional work towards various changes and improvements:

**Borderless fullscreen is now supported and made the new default.** This should improve window switching and multiple monitor support for all platforms.  
Because the window can now be resized dynamically, it is possible to toggle fullscreen by pressing F4 (screenshot is rebound to the printscreen key).  
The game now grabs your cursor when outside of menus, so your mouse cursor will not escape the window while playing in windowed mode.

Mice with more than 2 extra buttons are now supported.

There now is basic MIDI input support. This enables modders to use MIDI input devices (e.g. for music mods).  
MIDI input keys are also treated as regular keys so you can bind controls to a MIDI input key, in case you want to do [stupid things](https://www.youtube.com/watch?v=Ojcp8s35H6g).  
This is disabled by default. MIDI devices are enumerated in the console on start, after which you can set the `g_midiportin` autoconfig variable to your input device.

Text input should be more reliable in general, especially on Linux, where non-QWERTY keyboard layouts were poorly supported.

There were some other minor fixes for Linux: The window icon now shows up properly and the launcher window closes properly.