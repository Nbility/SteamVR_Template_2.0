﻿### Steam VR Template ###

Instruction guide [found in the onedrive]https://1drv.ms/f/s!AhConHxqM4Nisn-TFO1AtRNCJWhn

Disclaimer: The goal of this template is to put together a noob-proof SteamVR pawn to drop in your scene. However, one size for all solutions will not answer to all specific implementations, but it can gives you a head start. The template will be updated regularly with Unreal forum contributors suggestions. 

My eternal thanks to (but not only) @mitchemmc for input maps and controllers mapping and @PenguinTD for amongst many functions , teleportation method #2 and Ultraman.

Thanks to @mordentral for the grabbing fantastic plugin.

All assets are whether homemade, from the public domain or from Epic demos (you can use them freely in UE4 projects).

I remind everyone that any contribution is welcome. The commercial/fun value of VR projects is definitively not on who can use the Vive, who cannot. It's in the whole experience, the universe you are creating, the feeling, the originality and the user experience.

Have fun!

Mat, at Proteus VR


External credits:
* VRExpansion Plugin and functionnalities: @mordentral
* UltraMan: @PenguinTD

For questions,s see the forum thread: https://forums.unrealengine.com/showthread.php?106609-Steam-VR-Template 

# Version 2.0 – UE4.13.0: September 1, 2016 #

Changelog

* Oculus Rift compatible
* Now with parent/child blueprints
* Reconstruction of all functions
* Basic / Teleport / Grab / Specialized pawns
* VR Character, from VRExpansion plugin
* Choice of using or not using VRExpansion plugin
* Grab with/without the plugin
* Force feedback on objects
* Scalable mesh for Vive playground
* Robust teleport function on navmesh and/or safe normal value
* Teleportation with HMD and gamepad



#Features#

*	Basic Pawns and Character
*	Gamepad movement
*	Head mesh follow camera
*	Toggle base stations meshes (HTC Vive)
*	Oculus Rift user profile (Oculus Rift)
*	Access more VR functions (with the VRExpansion plugin)
*	Use a Character instead of a Pawn
*	Basic settings
*	Scalability settings
*	Teleport pawns
*	Controllers as animated hands or Vive Controllers (HTC Vive)
*	Selectable controllers’ skins & opacity (HTC Vive)
*	Mapping of all buttons/trackpad on controllers (HTC Vive)
*	Force feedback when touching objects (HTC Vive)
*	Go/No go teleportation zones with camera fade out
*	“UltraMan” mode
*	Triggerable poles at the 4 chaperone corners (HTC Vive)
*	Teleport on navmesh and/or adjustable "safe" value to teleport on uneven surfaces
*	No locomotion
*	Controller teleport and rotate playground with head position (HTC Vive)
*	Controller teleport center of playground only (HTC Vive)
*	HMD/gamepad teleport and rotate playground with head position
*	Controller movement
*	Grab pawns
*	Grab objects with/without the VRExpansion plugin
*	4 objects with skeletal sockets: the sword, the gun, the baton, the lightsaber; 1 object with mesh socket: the book; 1 object without sockets: the hat (with VRExpansion plugin) (HTC Vive)
*	Grab cubes (no plugin) (HTC Vive)
*	Vehicle pawn
*	Embark/disembark, drive vehicle (HTC Vive)
*	Platform pawn
*	Moving platform for testing purpose, by simple actor move (embark by triggering overlap volume or teleportation; disembark by teleportation) and sequencer (embark by pressing console button; disembark with controller input) (HTC Vive)
*	Jedi pawn
*	Turn on/off lightsaber (HTC Vive)


#Setup#
Files can be found [on OneDrive] https://1drv.ms/f/s!AhConHxqM4Nisn-TFO1AtRNCJWhn
GitHub version at https://github.com/ProteusVR/SteamVR_Template (you need to be logged to Github to open the link) 

To install as a template, just unzip into the appropriate templates directory like C:\Program Files\Unreal Engine[Version]\Templates for launcher version or[ForkLocation]\UE4\Templates for source version. 

Launch a new project, and you'll find it in the blueprint section.

To install as a project file, unzip in your usual projects folder. Then, delete the file SteamVR_x-x/Config/TemplateDefs.ini and you’re ready to go.

# IMPORTANT: If you open it like a regular project without deleting the .ini file, you’ll get errors messages.

To package your project:
Don’t forget to File/New C++ class, None, Create Class before packaging, if not the plugin won’t follow. Be sure to have a working copy of Visual Studio 2015 enabled.#   S t e a m V R _ T e m p l a t e _ 2 . 0  
 