# PPD Keyboard Remapper
Remaps PPD controls to be more suitable for keyboard play. I chose this layout after considering keyboard rollover that is a general limitation on laptop keyboards. In addition to remapping the keys, the script has a function to use the mouse as a slider. This script is meant to be used with GlovePie. You can also use it with a graphics tablet to play like in a real arcade. Use "0" and "9" by default to toogle the mouse lock. Pressing "8" will exit the script completely.

**What is Keyboard Rollover?**
----------------------------------------------------------------------------------------------------------------------------
Keyboard rollover is the ability of keyboard to correctly handle several simultaneous keystrokes. If pressing Q, W, and E in sequence without lifting your fingers from any of the three keys generates "QWE", the keyboard has 3-key rollover. This is important to consider because PPD requires at times 5 inputs at once. On laptops or some keyboards it is common to be unable to accept more than 3 keys. Distance from the keys may also be a factor. A keyboard may not be able to accept Q, W, E, and R at the same time. However, it may be able to accept Q, W, numpad 3, and numpad 4 at the same time. That is why I have settled for this control scheme, but it is possible to edit it to suit your perference.
               
**Configuration**
----------------------------------------------------------------------------------------------------------------------------
This script expects your configuration to be set to:  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Triangle = Left Shift  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Square = Z  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;X = U or numpad0  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Circle = I or numpadDot  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Arrow keys = Normal up, down, left, right  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Q = Left Slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;E = Right Slider  

   In addition to these mappings, the script will set the following bindings:  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Caplock = Left slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Numpad1 = Left Slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Numpad2 = Left Slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Numpad3 = Right Slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A = Right Slider  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;W = Up  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;S = Down  
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;D = Right
  
**Visuals**
----------------------------------------------------------------------------------------------------------------------------
This is a visual representation of what the key bindings should be. Do note that the keys will be numbered unlike this picture.

<img src="https://user-images.githubusercontent.com/100814612/158515541-1d314e36-7a3d-42af-a10c-695c57b85757.png">

This is the result of the script:
<p align="center">
<img src="https://user-images.githubusercontent.com/100814612/158518899-27df6551-49b0-4c6d-ab28-bc692acf11e5.png">
</p>
This is the layout we are trying to emulate. To have a slider like effect like the controller, we can use a touchpad or graphics tablet. For some, these options may not be available, so it is important that we set the keybindings in a way that the sliders are accessible to both hands. We do this in the above example.


<img src="https://user-images.githubusercontent.com/100814612/158713277-6a58193d-3169-49ed-b53d-983b13c7c167.png" width="600" height="300"/><img><img>

**Other Applications**
------------------------
With the new release of MegaMix+, it has come to my attention that having shift + numpad keys pressed at the same time can cause issues. Also, some games don't allow for caplock to be rebound. I have found a work around with these issues by rebinding the numpad keys and caplock (Numpad + shift keys will only be bound by what you set if numlock is toggled off which completely resolves the issues).

 ```
 //MegaMix+ Remapper (using default controls)

//Left Sliders
Keyboard.q = Keyboard.CapsLock
Keyboard.q = Keyboard.NUMPAD1

//Right Sliders
Keyboard.e = Keyboard.NUMPAD2
Keyboard.e = Keyboard.NUMPAD3

//Circle
Keyboard.l = Keyboard.NumPadDot

//X
Keyboard.k = Keyboard.NUMPAD0
 ```

**Summary**
-------------------
I understand that this project may be really niche and may not really help others, but I found it to be interesting. We look at the limitations in laptop keyboards and find a way around them. Now, could we bypass all of this by just getting a mechanical keyboard with built in remappable buttons? Yes, we could. But sometimes it's fun to see if there's an alternative.

**Other Related Projects**
----------------------------------------------------------------------------------------------------------------------------
[Macro Runner](https://github.com/Kttra/MacroRunner) - Run custom recorded macros on different gaming consoles and computers.

[TurboMode](https://github.com/Kttra/TurboMode) - Emulate the popular turbo mode feature from many custom controllers and arcade controllers.

[Stick Drift Fix](https://github.com/Kttra/Stick-Drift-Fix) - Stick drift is a prevalent problem in all types of controllers ranging from the switch to the playstation. This project prevents the controller from drifting at a software level.
