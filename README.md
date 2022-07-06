# Customized Mk3 v3.11.0: Stepper Motor Upgrades to Eliminate VFA's (Vertical Fine Artifacts)

<!--ts-->
   * Updates based on content from https://forum.prusa3d.com/forum/original-prusa-i3-mk3s-mk3-user-mods-octoprint-enclosures-nozzles/stepper-motor-upgrades-to-eliminate-vfa-s-vertical-fine-artifacts/
   * All updates from 'guykuo' v3.8.1 build, merged and retained 'KUO' Comment (https://github.com/guykuo/Prusa-Firmware/tree/0.9-Degree-Stepper-Support)
   * Additional updates made and 'CLX' Comment added
	* Stepper motors Variants (X&Y Axis)
     * Option 1: Moons MS17HA2P4100 0.9° steppers
     * Option 2: OMC-Stepperonline 17HM15-0904S 0.9° stepper
     * Option 3: Trinamic QSH4218-51-10-049 1.8° stepper (Increased Current Only)
   * Bear X-Axis - Sets Z_MAX_POS to 202 (8mm lower than factory X-Axis)
   * Extruders Supported
     * Skelestruder
     * Bondtech BMG Upgrade MK3/MK3S
   * Hotends Supported
     * E3Dv6
     * E3D Volcano
	 * Slice Mosquito/Magnum
   * Thermistors Supported
     * E3D_PT100
     * Slice HT (450C) 
   * MK3S/MK3S+ ONLY
<!--te-->

# Set Printer Variant
Use the correct variant file for your printer model. In Firmware/variants you will find several header (.h) files. Each printer model has one specific file.

Mk3s needs 1_75mm_MK3S-EINSy10a-E3Dv6full.h

Currently only MK3S and MK3S+ supported with this variant file.

Rename the variant file for your printer to be...

Configuration_prusa.h

Move Configuration_prusa.h to the main firmware folder.
-
PLEASE DO A FACTORY RESET WITH DATA ERASURE after installing this firmware. Failure to clear out old EEPROM setttings can produce odd printer behavior.
-
# Configuraiton / Compile / Load
For detail instructions reference Guykuo's github page for v3.8.1 at https://github.com/guykuo/Prusa-Firmware/tree/0.9-Degree-Stepper-Support

This update simply merges his changes into v3.11.0 and adds a few lines of support for Trinamic motors and Pruse Bear X-Axis update.