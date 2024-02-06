---
title: 3D Printers
---
3D printers build up objects out of melted plastic. We design the parts in [Onshape](/docs/software/onshape). From there, we use either one of our Stratasys printers or one of our Prusas to fabricate it.

TODO: add images to this tutorial
## Prusa
The 3 Prusa Mk3S+ printers are the workhorses of the Sigma Lab. Most parts should be printed on them. The process is fairly involved, so if you have any questions, don't hesitate to ask a teacher, TA, or classmate who knows what they're doing. They'll be happy to help. 

Here's how to print a part on one:
{{% steps %}}

### Export your model from Onshape.
In Onshape, right-click on the part you want to print and select Export. You should export it as a 3MF with Fine detail. 
### Open PrusaSlicer.
Open PrusaSlicer. If it asks you to pick which printer you have, select the Prusa Mk3S/Mk3S+ 0.4mm nozzle, then click Finish.
### Import your model.
Select the square with the plus, then select your downloaded .3mf file in the dialog that comes up.
### Orient your model correctly.
Using the move and rotate tools on the left side of the screen, orient the part in the way that leaves the fewest overhangs. This is a bit of an art, and you'll get a feel for it the more you print.
### Select the correct material.
In the upper-right corner, select the material you're printing. **_MAKE SURE THIS IS CORRECT, OR YOUR PRINT WILL FAIL AND MIGHT TAKE THE PRINTER WITH IT!_** If you don't know if you're printing in PLA or PETG or something else, ask someone.
### Select the profile.
In the same area, select the profile you want to use. It'll look something like `0.20mm QUALITY`. This is how you trade off between detail and printing speed. You'll get a feel for what you need as you get more experience, but a good rule of thumb is to use `0.30mm DRAFT` for parts you need quickly and `0.20mm QUALITY` for everything else.
### Slice the part.
Press the "Slice now" button in the bottom right of the screen.
### Fix the part if needed.
If PrusaSlicer throws an error, or the the print will take too long, or you'd like to otherwise change the print, click on the cube in the bottom-left of the screen and make tweaks.
### Get the approval of a teacher.
They'll make sure you haven't missed something that would cause the part to fail.
### Take the SD card out of an idle printer and plug it in to your computer.
You will probably need to use an SD to USB adapter.
### Press the "export to USB" icon in the bottom right of the screen.
Then save your file as a **descriptive filename**, preferably including your name and a version number. "Part Studio 1 - Part 1" *does not count!*
### Press the eject button in PrusaSlicer.
Then remove the SD card from your computer.
### Plug the SD card back into the printer.
The printer should beep and briefly show "Sorting Files."
### Select your file on the printer.
It should be the first one selected.
### Make sure the first layer goes down sucessfully.
This is a crucial step to make sure that if the part fails, it doesn't cause bigger problems. If class ends before the first layer finishes, ask somebody else to watch the print.

(For very large first layers, this step can be abbreviated, but make sure a teacher knows if you do this.)
### Check in on the printer periodically to make sure nothing goes wrong.

{{% /steps %}}

## Stratasys
This proccess is much more hands-off. Use GrabCAD print to slice, then send to the printer wirelessly.

## How to choose which printer to use
Prusa|Stratasys
---|---
Filament is cheap|Filament is a 10x markup
More control over the printer|More hands-off experience
Better for small, complex models with lots of overhang needing support|Better for large prints that don't need a ton of support