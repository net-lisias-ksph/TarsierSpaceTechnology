# Tarsier Space Technology

* 2016-0401: 5.9.1 (JPLRepo) for KSP 1.1 PRE-RELEASE
	+ This is first cut experiments pre-release for upcoming Full release when KSP 1.1 goes full release.
	+ BEWARE: This no doubt has BEES in it, and is NOT a RELEASE version.
	+ Please report all bugs on github. The more eyes on it, the better it will be when 1.1 releases.
* 2016-0327: 5.9 (JPLRepo) for KSP 1.1
	+ Fixed TST AppLauncher Icon appearing in map view even when active vessel has no TST parts.
	+ Fixed error on start-up for integration with Kopernicus mod.
	+ Fixed KIS/KAS support for the small Science Drive.
	+ Massive re-factor of the code base for future ease of maintenace support and preparations for KSP 1.1 (THIS DOES NOT mean TST is ready for KSP 1.1).
	+ Added additional Space Telescope part config file parameters for future integration with other telescopes (like DMagic's Orbital Science).
	+ Fixed the TST icon showing sometimes when it shouldn't (Tracking Station, In Flight Map mode, when active vessel has no TST parts on it).
	+ There is now a Settings menu available from the SpaceCenter so you don't have to edit the config file directly.
	+ Settings you can change:
		- If you try to make any of these settings larger than your screen size TST will automatically cap it. If you set it too small, bad luck, change it back to a larger value.
		- The size of the ChemCam camera window for both small and large size setting (in pixels).
		- The size of the Telescope's camera window for both small and large size setting (in pixels).
			- Use Stock App Icon" - if ON will use the Stock App Icon AppLauncher button, if Off will use Blizzy's toolbar.
		- (requires you to change scene for this setting to take effect, eg: go to Editor, Flight, TrackingCentre, etc).
			- Debug Logging ON" - This will turn debugging messages in your output log ON or OFF. Leave it OFF (As it causes performace issues) unless you are having some problems with TST, then turning it on and capturing your log and sending to me greatly helps me to help you.
		- ToolTips - Yes the GUI windows now have Tooltips - you can turn them on and off here.
* 2016-0127: 5.8 (JPLRepo) for KSP 1.0.5
	+ V5.8 Added support for ResearchBodies mod (MUST HAVE ResearchBodies V1.6 or above).
		- If ResearchBodies mod is installed then:-
		- Telescope and ChemCam contracts will NOT generate for bodies that have yet to be discovered.
		- If you take a picture with a Telescope of a body that is yet to be discovered AND transmit/recovery it, it will become discovered.
		- Subsequent pictures taken and transmitted/recovered of a already discovered body will add 20 research to that body.
		- The TST Telescopes act the same as the ResearchBodies telescope, IE:they have the Research button in their right click menu and will discover bodies they are pointed at in the same way as the ResearchBodies telescope does.
		- The TST GUI camera-window "Show Bodies" list will NOT show un-discovered bodies or galaxies.
		- V5.7 Completing TST telescope picture contracts will no longer register in a career game as having Reached that body. This was interfering with KSP generating the default
			- flyby and explore contracts for the bodies.
* 2015-1112: 5.6 (JPLRepo) for KSP 1.0.5 Silent Edition"
	+ Updated for KSP 1.0.5 including adding support for new Science transmission failure feature to put science back into telescopes and drives when transmissions fail.
	+ This version is only compatible with KSP 1.0.5, do not upgrade KSP 1.0.4 installs with this version.
* 2015-1031: 5.5 (JPLRepo) for KSP 1.0.4.
	+ V5.5 Amended support for Distant Object Enhancement mod and Remote Tech mod so that TST no longer is bound to a specific version of these mods.
		- From now on TST should work with any version of DOE and RT. Reminder: DOE support for flares should now work. RemoteTech : TST parts and menu only works if you have
		- local control or active connect for a vessel.
		- Added Science Defs for Real Solar System and Outer Planets Mods. Science defs and contracts as well as all of TST should now fully support RSS and OPM. NB: To use the science defs
		- for RSS and OPM you MUST have Module Manager mod installed.
		- ChemCam contracts will now only offer/allow up to x active or offerred contracts (before was unlimited). x by default is 3. You can change this in the Config.cfg file field "maxChemCamContracts".
		- ChemCam contracts will now only be offered for bodies you have already photographed using a Telescope by default. You can change this in the Config.cfg file field "photoOnlyChemCamContracts".
		- Externalised lists of bodies and galaxies now in the config.cfg settings file, these lists determine the order (and if) a Telescope/ChemCam contract will be offerred.
		- The TSTGasPlanets node in the config file is a list of gas planets that are excluded from all ChemCam contracts, Can't land on a gas planet can we!
		- The TSTStockPlanetOrder node is the valid and order of bodies and galaxies contracts will be offerred for Telescope contracts. For ChemCam contracts a random body is selected from this list based on the prestige level
		- you have already completed a ChemCam contract for (As per previous comment about prestige levels for ChemCam contracts).
		- The TSTRSSPlanetOrder node is the list used if you have Real Solar System mod installed (ignored if it is not installed), operates the same as the TSTStockPlanetOrder list described above.
		- The TSTOPMPlanetOrder node is the list used if you have Outer Planets mod installed (ignored if it is not installed), operates the same as the TSTStockPlanetOrder list described above.
* 2015-0718: 5.4.1 (JPLRepo) for KSP 1.0.4.
	+ Support for KSP 1.0.4. Attempting the impossible to improve the camera wobble in a 32bit Game engine where floating point errors are inevitable and a losing battle with what is called 'spatial jitter'.
	+ Have added Gyroscopic ReactionWheels to the Space Telescope parts.
	+ Have added a Button in the TST menu labeled "F/T" that appears to each space telescope.
	+ Pressing this button will bring up a fine tuning window that allows you to:
	+ Fine tune the Gyroscopic ReactionWheels "Sensitivity" (default=1) and "Powerscale" (default=0.10 torque) using sliders.
	+ Have added fine tuning of the SAS PID controller "KP (default=12), KI (default=6), KD (default=0.5)" values through three sliders on the same window.
	+ If you don't know how a PID controller works or these values you can start reading up here.
	+ https://en.wikipedia.org/wiki/PID_controller
* 2015-0623: 5.4 (JPLRepo) for KSP 1.0.3
	+ support for KSP 1.0.3
	+ Seems improvements in KSP 1.0.3 have made the camera wobble better (but not perfect).
* 2015-0613: 5.3 (JPLRepo) for KSP 1.0.5
	+ Fixed GUI issue with Critical Temperature gauge mod.
	+ Saved camera pictures now in TWO sizes. Low and high(full screen) res. - Also added save camera pictures to the ChemCam part (previously only telescopes could save pics).
	+ Fix to take picutre/fire laser messages to provide feedback on science collected/not collected AND pictures saved.
	+ Now compatible with Kopernicus planet mod.
	+ Toolbar and/or Applauncher buttons (and GUI) now only show if you have TST parts on the active vessel.
* 2015-0602: 5.2 (JPLRepo) for KSP 1.0.5
	+ Added check for local control for Remote Tech.
	+ This is not save game breaking from V5.0 up.
* 2015-0601: 5.1 (JPLRepo) for KSP 1.0.5
	+ Remote Tech support for new GUI window. Now if no connection you cannot open/close cameras, view science or move science to SDDs.
	+ Re-sized the new GUI window to make it a bit bigger.
	+ This version will not break save games from version 5.0.
* 2015-0529: 5.0 (JPLRepo) for KSP 1.0.5
	+ Added Menu (GUI) that can be opened/closed via the stock AppLauncher or Toolbar by Blizzy.
	+ Menu shows telescopes, chemcams and SDDs on vessel. Allows you to open/close cameras, Camera GUI, fill SDDs and view science directly from the GUI.
	+ Added Menu items to camera screen to view Celestial Bodies (just like the Galaxy list) so you can set camera target from the list.
	+ Added Action Menu support for open/close cameras and fill SDDs.
	+ Added Distant Object Enhancement mod support.
	+ Added a Config file with the following Settings:-
	+ FwindowPosX,Y - X and Y position for the new GUI window.
	+ CwindowPosX,Y - X and Y position for the Telescopes/ChemCam Camera GUI window.
	+ GalwindowPosX,Y - X and Y position for the Galaxy list window.
	+ BodwindowPosX,Y - X and Y position for the Celestial Bodies list window.
	+ ChemwinSml, Lge - ChemCam Window Size in pixels for both small and large window. (can now toggle small and large windows for the ChemCam just like the Telescope camera GUI).
	+ TelewinSml, Lge - Same as the ChemCam Window size but this is for the telescope camera GUI.
	+ UseAppLauncher = true / false - if True uses the in-game Application Launcher buttons for the new Menu GUI. If set to false, will use Toolbar by Blizzy (optional separate mod install).
	+ debugging = False / True - Turns on/off Log Spam for debugging purposes.
* 2015-0509: 4.7 (JPLRepo) for KSP 1.0.
	+ Added KAS and KIS support for the small HDD(SDD) - Requires Module Manager to be installed.
	+ Can now STORE science data into SDDs via EVA. Reminder Warning: Storing and removing science data from SDDs lose some science value each time (data corruption feature).
	+ Drive Capacity for SDDs upped to 120mits (about 4 pictures) and 480mits (about 16 pictures).
	+ Re-balance max temperatures of parts.
	+ The Small Telescope now only returns 80% of max science value for pictures of planetoids and 50% of max science value for pictures of galaxies. The Large Telescope returns Full science value.
	+ Added Science descriptions for the Galaxies.
	+ Added lab boost to Science gathered - science can now be boosted in the Mobile Lab.
	+ Added KSP-AVC support.
	+ Converted all PNGs to DDS files now supported in KSP 1.0.x.
* 2015-0502: 4.6 (JPLRepo) for KSP 1.0.0
	+ Compat. with KSP V1.0.0
	+ Rebalanced all parts costs and to new Tech Tree.
	+ nerfed Small telescope range.
	+ Fixes for contract spamming and you now need the Large telescope Tech for the Galaxy contracts.
* 2015-0213: 2.5 (JPLRepo) for KSP 0.7.3
	+ Fixes for 0.90
	+ Fixed to integrate with Autopilot correctly.
	+ Fixed for contracts and galaxies to work correctly.
* 2014-0710: 2.5 (tobyb121) for KSP 0.7.3
	+ Got rid of camera wobble!!!
	+ Added a new telescope and tweaked the zoom to fit into the tech tree
* 2014-0110: 2.4 (tobyb121) for KSP 0.7.3
	+ Telescope:
	+ Servos added for fine control
	+ Extra info displayed on what telescope is looking at
	+ Can collect science from EVA
	+ Hard Drives:
	+ Removed limitations on HDDs which only allows 1 item per science subject, now unlimited
* 2013-1228: 2.3-VE (tobyb121) for KSP 0.7.3
	+ No changelog provided
* 2013-1227: 2.3 (tobyb121) for KSP 0.7.3
	+ Added targeting to TelescopeCamera
	+ Bug fixes for performance
* 2013-1223: 2.2 (tobyb121) for KSP 0.7.3
	+ Fixed low FPS when camera closed.
	+ Created release build for extra performance.
* 2013-1222: 2.1 (tobyb121) for KSP 0.7.3
	+ Correct part.cfg files instead of test ones.
* 2013-1221: 2.0 (tobyb121) for KSP 0.7.3
	+ Added space telescope and fixed science hard drives to work with KSP v0.23
* 2013-1029: 1.1 (tobyb121) for KSP 0.7.3
	+ Fixed part config files
* 2013-1027: Science Hard Drives (tobyb121) for KSP 0.22
	+ Initial Tarsier Space Tech release, contains science hard drives
