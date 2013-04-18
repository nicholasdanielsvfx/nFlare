I will no longer be supporting this repository,and will be revisiting the setup to address issues involving more advanced features of flares. Hope you all understand, and enjoy the script! 
=
- Nicholas
=
---

nFlare - Nuke Gizmo
=
`This node's goal is to create flares faster and more optimally, based on premade Flare nodes.`

---
## Getting Started on Windows 7
Locate the directory to which all of Nuke's gizmos, Toolsets, scripts, etc are saved.	
This is typically located at: `C:\Users\%USERNAME%\.nuke`	

* Don't be afraid to be adventurous in using another folder to store your Nuke-related items. For instance, I have my setup on a separate drive that I can swap between desktops, or direct to a location on a server so multiple computers can accses.

Go ahead and open up a command line and type in:	
`setx NUKE_PATH C:\Users\%USERNAME%\.nuke /m`	
The magic you just did was create a system environment variable that allows Nuke to access a location in which this node will store important preset information.
###### Access via GUI
For a GUI approach, or to see what you just did, just open up an Explorer window, right click on 'Computer' and select 'Properties'. From there, click on 'Advanced System Settings' > 'Advanced' Tab and click on 'Environment Variables...'.	
In this window you can see the User variables and System variables, in which you can create a new variable by inputting the name `NUKE_PATH` and value `C:\Users\%USERNAME%\.nuke` respectably, and you're good to go!

* Keep in mind that at this time there is a fail-safe that if the system variable is not set, that it defaults to `C:\Users\%USERNAME%\.nuke` or wherever your menu.py may point to, thus saving presets in that location.

## How To Use
Upon downloading from git, copying from source, or retyping it all in the same sense, the idea of implementation is to add the .nk file to the Toolsets directory designated by the NUKE_PATH environment variable.

The ideal folder structure of your .nuke folder should at least include:	
* assets
* Toolsets

In which case, it would be best for organizational purposes to drop the .nk file into the Toolsets folder, as it is essentially a group rather than a gizmo. 

However your setup is at home, whether you manually code change your menu.py or you have a script that automagically reads all the toolsets and gizmos into Nuke. It's as simple as hitting Tab and entering in 'nFlare_v#'.

Upon node generation, you can start pushing away at creating flares from the list of premade flares of different types.	
After you create a flare you like, you can save the preset by pressing the 'Create Preset' button, and enter a name when prompted. The file will be stored in the location set by the environment variable `NUKE_PATH` or to Nuke's default.
* At this time it is advised not to create any presets that start or end with a 't' or 'n', as these currently cause issues with the python script.

## Requirements
Has been tested on equipment using
* Windows 7
* Nuke 6.3v4

## Current Status
* Proceed with tests on Mac & Linux
* Proceed with tests on other versions of Nuke
* Investigate feasibility of icons
* Aim to implement into a gizmo format (User tab generation issue)
* Global color options

## Contact
#### Creator

[Nicholas Daniels](http://github.com/nicholasdanielsvfx)  
[Website](http://www.endyarts.com)  
[Email](mailto:endyarts@gmail.com)

