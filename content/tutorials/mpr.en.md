---
title: MPR and 3D cursor
weight: 80
description: How to use Multiplanar reconstruction (MPR) and 3D cursor (crosshair)
keywords: [ "mpr", "multiplanar reconstruction", "3d cursor", "open source dicom viewer" ]
---

## <center>MPR and 3D cursor (crosshair)</center>

### Orthogonal multiplanar reconstruction (MPR)

The orthogonal multiplanar reconstruction (MPR) allows to create, from the original plane (usually axial), images in the two other planes of the Euclidean space. Only planes along the 3 axes (x,y,z) can be displayed, an oblique plane cannot be obtained with this tool.

The MPR view can be opened with {{< svg "static/tuto/icon/mpr.svg" >}} in the toolbar or by right-clicking on the thumbnail in the [DICOM explorer](../dicom-explorer/).
{{% notice note %}}
The menu and the button are only active if the series contains at least 5 images.
{{% /notice %}}

When the tab containing the MPR views is selected, the crosshair tool {{< svg "static/tuto/icon/crosshair.svg" >}} is automatically applied on the left mouse button. Note that it is possible to change the window/level with the [ctrl key](../../basics/shortcuts/) while keeping crosshair selected.

{{% notice tip %}}
Once the 2 new plans are created, they also appear in the [DICOM explorer](../dicom-explorer/) and can be [exported](../dicom-export/#dicom-export).
{{% /notice %}}

![QuMPR](/tuto/mpr.jpg?classes=shadow)
<br>

{{% notice info %}}
For more information on the elements related to the orientation of multiplanar views see [MPR orientation](../image-orientation/#orientation-in-2d-multiplanar-reconstruction-mpr).
{{% /notice %}}


### 3D cursor (crosshair)

The 3D cursor allows you to synchronize the position of several views sharing the same 3D coordinate system.

In order to know which series sharing the same coordinate system, you can select more than one series from the DICOM explorer by right-clicking on a series and selecting "_Select related Series_". Then open the series selection by right-clicking again and selecting "_2D Viewer > Open_"

The crosshair tool {{< svg "static/tuto/icon/crosshair.svg" >}} can be selected in the mouse buttons on the toolbar or by right-clicking on a view.


![3D Cursor](/tuto/3d-cursor.jpg?classes=shadow)
<br>


### Preferences

From the menu "_File > Preferences > Viewer > MPR_" (Since {{< badge "v4.1.0" >}}):

* _Auto center axes_: allows to choose a behavior to recenter the cursor in the different views. The position can be returned to the center systematically with the "Always" option (see the image above) or with the 2nd option only when the position is almost no longer visible (the default value).
* _Crosshair gap at the center_: defines the size of the empty space in the center of the crosshair.


{{% notice info %}}
The preferences apply to both the MPR and the 3D cursor.
{{% /notice %}}