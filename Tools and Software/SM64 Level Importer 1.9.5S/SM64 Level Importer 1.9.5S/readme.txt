SM64 Level Importer 1.9.5S by Skelux
Versions 1.6 and earlier by messiaen (frauber)

You may refer to these links for the latest downloads and documentation:
http://origami64.net/
http://sites.google.com/site/messiaen64/level-importer

YouTube channels:
http:/youtube.com/user/skelux
http:/youtube.com/user/frauber

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
*Normals are imported into the level (sketchup pro exporter needed)
*Level models are perfectly centered
*Increased water box, death height limits
*Automatic correction of Mario shadow size (TT64 shrinks it)
*Various less noticeable changes