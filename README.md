# GSX Profile for EDDH Hamburg Airport.
this is a GSX Profile for the payware Simwings EDDH Scenery airport. 

Profile includes walking paths, and adjusted vehicle positions, corrected Parking positions and sizes and GSX VDGS panels, that override the non functional ones from teh scenery.
The Main Gates 1-8 use APIS Panels, the Gates 9-12 Use T1S-42 and T2S-42. I tried to match the present VDGSs as close as possible.
The stop positions were adapted but may need some further work.

I added a replacement option for Ground Services. Sadly I did not figure out how to add new Ground Handlers fro scratch however I added an Option to replace 
HAS (Hong Kong Airport Services Limited) so that they appear as Hamburg Airport. (memory hook: HAS as Hamburg Airport Services)
I know it is not the HMA Ground Logo but that would be way to small on the vehicles and not match the sceneries stairs.
See installation for more information and limitations.

## Features  
### Gates  

- Gate 1-8 (A/B): 
  - custom Positions
  - APIS
  - Jetway Paths
  - Terminal Paths
- Gate 1-12: 
  - custom Postitions, 
  - Safedock T1S-42, 
  - Walking paths
- Gate 81-88: custom Postitions, 
  - Safedock T1-42, 
  - Waling paths
- Gate 91-95 (A/B): 
  - custom Postitions, 
  - Safedock T1-42, 
  - Walking paths
- Gate 47,47: 
  - custom Postitions
- Parkings were not edited

### Ground Hanlder
- Hamburg Airport Ground Services Livery Replacement


## Known Issue:

Some Gates were found to be missing because there are no Parking Positions present:  
Gate 1, Gate 2, Gate 5, Gate 3, Gate 4, 


For Users that use the Simwings / Aerosoft Scenery from the In-Game Marketplace the scenery may not be recognized correctly by GSX.  
To fix this issue the AFCAD file needs to be placed in the GSX Profiles path:
`\Users\<username>\AppData\Roaming\virtuali\GSX\MSFS\eddhswairport.bgl`
since I could not find any scenery file im the Maketplaces files I needed to get it from the 3rd Party download variant.  
the file can then be found:  
`\simwings-airport-eddh-hamburg\scenery\simwings\EDDH\eddhswairport.bgl`

sadly I can not include the file her due to copyright reasons but there are places to look or kindly ask a friend.

## Installation:

To install, extract the .zip and move the "eddh-simwings.ini" file inside to the following route:  
`\Users\<username>\AppData\Roaming\virtuali\GSX\MSFS`

Replace the HAS Livery Textrue file by overwriting it in the GSX (Addon Manager) Installation directory.  
`<path>\Addon Manager\MSFS\fsdreamteam-gsx-world-of-jetways\SimObjects\GroundVehicles\FSDT_Staircase_TLD_ABS-580\texture.HAS\GSX_LOGO_4X1.PNG.DDS`
This Installation needs to be refreshed after every GSX update

To remove the HAS Ground Handler replacement:
open "eddh-simwings.ini" in notepad++ and find and replace:

find:        handlingtexture = HAS
replace:     handlingtexture = 
search mode: normal

To remove GSX VDGSs and use the simwings sceneries ones:
open "eddh-simwings.ini" in notepad++ and find and replace:

find:        ^.*ApisLsupport|ApisWall|SafeDockTS42|SafeDockT42|SafeDockTS24.*$
replace:     Dummy
search mode: regular expression


Editing and reupload is explicitly permitted.