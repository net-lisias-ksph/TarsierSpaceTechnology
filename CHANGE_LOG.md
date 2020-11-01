# Tarsier Space Technology

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
