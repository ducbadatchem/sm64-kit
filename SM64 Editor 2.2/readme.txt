SM64 Editor Version 2.2 by Skelux
Versions 1.6 and earlier by messiaen (frauber)

A copy of the extended OBJ plugin for Blender can be found in 'Data/Patching Tools/io_scene_extended_obj.rar'.
You may refer to these links for the latest downloads and documentation:
http://origami64.net/
http://sites.google.com/site/messiaen64/level-importer

YouTube channels:
http:/youtube.com/user/skelux
http:/youtube.com/user/frauber

Changes in 2.2:
*Support for extended OBJ format
*Support for vertex shading

Changes in 2.1.4:
*Minor bug fixes

Changes in 2.1.3:
*Further improvements to patching process
*Moved around some banks which weren't listed in the RAM map
*Fixed importer sometimes getting stuck infinitely importing the model

Changes in 2.1.2:
*Added option to reset ROM patches on misc tab
*More-efficient patching process
*Fixed patching order errors which may affect fresh ROMs
*Fix menu, Mario, and title skip tweaks to work on real hardware
*Updated RAM map

Changes in 2.1.1:
*Reverted byte-aligned bank patching for now, seems to cause issues

Changes in 2.1:
*Increased space for level models (non-custom entry point)
*Added option to ignore level size limit (be careful!)
*Added option to import to custom location
*RAM is set up for infinite polygons (emulator hacks needed above 8MB, collision still limited)
*Functionality for building a fresh level script when necessary
*Neater ROM patching process
*Removed texture and vertex limits
*Patching process aligns banks properly
*Opaque layer uses N64-compatible 0xFC command for non-fog

Changes in 2.0.9.1:
*Fixed bugged sequence extracting

Changes in 2.0.9:
*Freed up more space for custom sound importing (you'll need to re-select instrument sets and song names)
*Fixed broken "Mario (Ext.) - Bottom" preset, re-apply the 0x04 bank extender tweak to fix your ROM
*Music table can be re-built dynamically, this will be used for custom music table building.
*Updated RAM/ROM map

Changes in 2.0.8:
*Added tweak for extended bank 0x04, and custom import presets which use the extra space for Mario's model
*Death floor still works if you didn't extend the boundaries

Changes in 2.0.7:
*Fixed reading textures for models made in Blender and other programs
*Allocated music data 0x807C0000 when music hack disabled (best compatability), 0x803D0000 when enabled
*Fixed SFX in final Bowser stage, caused by allocation of music data in RAM
*Fixed two incorrectly labelled music tracks

Changes in 2.0.6:
*Fixed scrolling textures not being removed correctly in the ROM
*Fixed level lists not being cleared after importing a level

Changes in 2.0.5:
*Fixed a drawing-distance issue which would cause distortions i lookon real N64 hardware

Changes in 2.0.4:
*Fixed fog not working for newer SketchUp models
*Fixed reading diffuse for Blender models
*Fixed reading models with no UV mapping
*Improved image processing speed
*Improved scaling of alpha layer

Changes in 2.0.3:
*Fixed sometimes getting stuck in a permanent loop while importing
*Fixed incorrect naming of imported sequences
*Prettier icon

Changes in 2.0.2:
*Corrected a RAM issue which would cause crashing in some ROMs
*Added a tweak for disabling the CRC
*Fixed CRC sometimes not updating
*Reduced size of converted display lists

Changes in 2.0.1:
*Sequences as large as 0x24000 are now supported (twice the previous limit)
*Sequence data relocated in RAM to allow for larger collision data
*Fixed incorrect reading of diffuse resulting in a crash

Changes in 2.0:
[Model Conversion]
*Transparency is fully functional, use the sliders in SketchUp
*Refractive surfaces can be enabled by adding "_ref" to a material name
*Custom backgrounds are automatically resized and imported seamlessly
*Improved efficiency and speed of display list conversion
*Support for a large range of texture sizes (16x16, 8x32, 64x4, etc)
*Added automatic resizing of all incompatible texture dimensions
*Support for faces with no texture image, only a color
*Drawing layer in custom importer is chosen automatically
*Enabled death floors for custom importer
*Fixed importing of indexed textures
*Fixed some models not being centered correctly
*Fixed importing models which contain no opaque textures
[Music]
*Added ability to open Mario Kart 64 (U) ROM files and import music
*Added support for note velocity, MuseScore 2 recommended
*Added reverb setting for channels in XML converter
*Extracted sequences are also converted to a MIDI, incomplete
*Fixed low-pitch notes in XML converter
*Added option for sequences to play while the game is paused
*Fixed a bug with duplicate track names
[Interface]
*Imported level names are stored in the ROM
*Added Windows 10 support
*Various improvements to error-handling and interface
*Fixed reopening the same ROM/obj not re-reading the file
*Fixed mislabeled level/song names throughout the importer
*Fixed log files not displaying correctly in notepad
[Misc]
*Replaced M64 ROM Extender and rom_expand_64.exe with queueRAM's sm64extend.exe
*Enabled negatives for floats in the tweak editor
*Format of "Offset Polygon" property of scrolling textures starts at 0 instead of 1

Changes in 1.9.5S:
*Fixed error handling on collision tab
*Fixed incorrect patching of Mario's shadow size/opacity
*Fixed PPF pointlessly modifying the Whomp King's star spawn location
*Included the updated RAM_map.txt
*Moved extended music data to 0x805C0000 for better compatibility

Changes in 1.9.4S:
*Added option to ignore level size limit by holding alt-clicking 'Import Level'
*Improved navigation in collision editor
*Collision types are saved automatically
*Reorganized RAM usage and updated RAM map
*Three new tweaks by Kaze
*Fixed various mislabeled instruments
*Relocated scrolling texture routine to 0x1202400/0x80402400
*DMA copy code at 0x101B84 is only written after the first import
*Fixed custom importer's maximum offset ignoring the alpha display list size
*Removed bugged option of reverting title screen
*Various minor improvements to interface

Changes in 1.9.3S:
*Fixed minor graphical errors caused by increased clipping distance
*It is recommended to re-import levels created in 1.9.2S
*Fixed crashing separate collision in custom importer
*File dialogue goes to last known directory if location is missing

Changes in 1.9.2S:
*Increased 3D draw distance, no clipping in large levels
*Significant improvements to tweak syntax, you may need to manually update old tweaks
*Collision types work when importing without textures
*Enabled importing of alpha textures in custom importer
*Added three new water types
*Tweaks for changing cap music also fix the music in their corresponding level
*Tweak for changing ROM internal name
*Custom importer allows more space for title screen importing
*Fixed miscalculation causing custom BG to overwrite other levels
*Fixed miscalculation of bank 0x0E size
*Fixed slight misalignment of texture mapping
*Fixed collision not being centered in custom importer
*Fixed model offset position in custom importer
*Fixed incorrectly labeled music sequences
*Fixed mislabeled instruments and collision types
*Fixed bug in maximum size for custom importer
*DMA copy code at 0x101B84 is not rewritten every import
*Four new tweaks by Kaze
*Improved efficiency of display list conversion
*Further improvements to interface

Changes in 1.9.1S:
*Allowed importing of a separate model for collision
*Added the option to apply a tweak automatically after importing
*Increased RCVI hack from 3x to 4x regular
*Reversed a change in display list conversion which would increase size
*Six new tweaks created by Kaze
*Minor changes to interface

Changes in 1.9S:
*Added custom model importer and various presets
*Added tweak manager and various tweak files
*A basic hex editor is included in the miscellaneous tab
*Flawless obliteration of all stretched textures
*Removed polygon limit, though results may be unstable
*Skipping of opening has been moved in to the tweak manager
*Star requirement editing has been added to the tweak manager
*Can disable messages displayed after collecting certain amounts of stars
*Fixed loading of settings in 'Level Settings' tab
*Fixed collision parameter descriptions
*Updated collision type descriptions
*Fixed music silence bug which was incorrectly fixed in earlier versions
*Added palm tree to default geometry layouts
*Fixed conflicting model ID on TTM and RR 0x0E object banks
*Changed default import level to Bob-Omb's Battlefield
*Added option not to center the model
*Removed texture scale setting
*Minor interface improvements
*Improved efficiency of display list conversion

Changes in 1.8.1S:
*GUI background fixed for widescreen displays
*Error handling for write-protected MTL file
*Handling of various minor errors
*Explanations of scrolling textures when labels are clicked
*Mist and toxic haze is displayed correctly
*Multiple water boxes display correctly
*Added option to create invisible water boxes
*Added texture scale option for water boxes

Changes in 1.8S:
[Model Conversion]
*Scrolling textures have been added to the Special Material tab
*Death floor extends beyond original boundaries
*Fog works on alpha textures
*Experimental transparency option
*Most stretched textures are corrected automatically
*Vertices exceeding the maximum range are corrected
*Added texture scale option
*Shading options are numeric
[Music]
*Supports up to 70 music sequences
*Descriptions of each instrument set added
*Music XML Converter incorporated into program
*High notes are shifted down octaves until valid
*Chords are imported almost perfectly
*Added Vibrato setting for each channel
*Can select the percussion channel from instruments list
*Selected instrument set is saved to file and recalled when importing
*Channels 10 to 15 are working
*Working pitch and transposing options
*Fixed music volume problem with certain sequences
*XML containing notes of 1/128 length or less import correctly
[Interface]
*Improved aesthetics
*Simplified directory structure
*Last directory for each dialog is saved
[Memory Banks]
*Bank 0x0E objects are working in levels of any size
*Overriding music size restrictions should not interfere with maximum level size
[Misc]
*New Easter Eggs added
*Added option to enable extended boundaries
*Added a PPF applier to the Misc Settings tab
*SM64 ROM will be automatically patched if not prepared for importer
*An incorrectly prepared ROM can be opened but importing is disabled
*CRC is automatically corrected
*Added an incomplete text editor
*Fixed bug causing trajectory to occasionally read incorrectly
*Added option to disable level intros
*Added option to enable widescreen improvements
*Main patch file does not alter credits
*Included many sample sequences

Changes in 1.7S:
*Support for up to 20,000 polygons
*Roms are extended to 64mb
*Option to enable VC hack to solve lag
*Normals are imported into the level (SketchUp pro exporter needed)
*Level models are perfectly centered
*Increased water box, death height limits
*Automatic correction of Mario shadow size (TT64 shrinks it)
*Various less noticeable changes