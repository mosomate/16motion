# 16Motion
Configurable, 3D printable carriage for aluminium extrusions. A 16Motion carriage consists of four 3D printed plates put together around the extrusion and some **cheap**, **easily sourceable** hardwares including 684 bearings, M3 and M4 screws and nuts.
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://raw.githubusercontent.com/mosomate/16motion/main/docs/cover.png)
# Disclaimer
As steel bearings are rolling on aluminium, they might leave marks and/or wear out the extrusion over time. For **casual** usage it's not significant, but for **regular** usage you should consider using lubrication (ex. a thin layer of lithium grease should do the job).

This design is sensitive for dirt building up on the extrusion. Wiping them clean before usage is recommended!

If you can accept these conditions, then have fun building your carriages!
# BOM for one plate
For one of the four plates you need:
- 3D printed plate **x1**
- 3D printer bearing spacer **x4**
- M4x(width of extrusion + 10 mm) screw **x2** *(ex. if the extrusion is 20 mm width, screw length will be 20 mm + 10 mm = 30 mm)*
- M3x16 screw **x2**
- M3 self-locking nut **x2**
- 684 bearing **x4**
# Precompiled STLs
I uploaded precompiled STLs to Thingiverse for **20 mm**, **25 mm** and **40 mm** wide extrusions. Check them out [HERE](https://www.thingiverse.com/thing:6853255). If you can't find the suitable sizes to satisfy your needs, then proceed with the customization.
# Customization and assembly
You can find here the necessary steps for customizing the plates and assembling the carriage. Each step has a video tutorial of it, click on the banner to watch them on YouTube!
## Plate customization
- Open **FreeCAD** and open **Plate.FCStd**
- If you see nothing but the model of a ring (spacer) you have to toggle the visibility of the plate. Right click on **Plate** object and select **Appearance...**. Then open the dropdown at **Document window** and select **Flat Lines** again
- Right click on the **Plate** document and check **Skip recomputes**
- Click on **Spreadsheet** and edit the **Ideal extrusion width** and **Actual extrusion width** parameters. **Ideal extrusion width** is the theoretical width of one side of the extrusion (e.g. 20 mm) and the **Actual extrusion width** is the masured size of it (e.g. 19.9 mm). For maximum accuracy I recommend using a caliper for measuring
- Right click on **Spreadsheet** and select **Recompute object**
- Recompute all remaining objects as well (Plate, Spacer and Assets)
- Select **Mesh** from the Workbench selector
- Select **Plate** object by clicking on it and click on **Create mesh from shape...** button. My preferred settings for mesh creation are: **Surface deviation => 0.1 mm** and **Angular deviation => 5.00 ˚**
- Create mesh from the **Spacer** object as well
- Export meshes by right click on them and select **Export mesh...**

[![Plate customization video](https://raw.githubusercontent.com/mosomate/16motion/main/docs/plate_customization_banner.png)](https://www.youtube.com/watch?v=9Bi0MCfb9tI "Plate customization | 16Motion Video Series")
## Plate assembly
- After 3D priting, drill an M4 thread into the **bottom left** and **top right** holes
- Insert an **M3 self locking nut** into the socket below one of the tension levers
- Insert an **M3x16** screw through the tension lever and drive it until it barely touches the lever
- Repeat the step above for the other lever

[![Plate assembly video](https://raw.githubusercontent.com/mosomate/16motion/main/docs/plate_assembly_banner.png)](https://www.youtube.com/watch?v=31CdhINwxhE "Plate assembly | 16Motion Video Series")
# License
Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg