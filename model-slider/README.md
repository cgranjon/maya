# Main Command (MEL)
source "cg_modelSlider.mel";


# How to install
Save the script in your "../maya/../scripts/" directory.

# How to use
1. In Maya, select a model you want to line up (select in the viewport, not the Outliner. The tool needs an active viewport.)
2. Make sure the camera has an imagePlane.
3. To launch the tool, use the following command in a shelf button: source "cg_modelSlider.mel";
4. Use Ctrl+MMB Drag over the "Depth" value to gradually reveal or hide the imagePlane. The "Sliding Precision" parameter will make the Ctrl+MMB Drag more or less sensitive, which is helpful for lining up small details.

# Notes
1. When adding a new camera to the tool, the user must select the model through another modelPanel (i.e. have an other active viewport).
2. Using the command from the Script Editor will not work because the Script Editor will take the focus. We need a viewport to have the focus (grey line around the active window.)

# Why this tool ?
This tool is designed to help a modeller compare a model to a reference image. Lining up models by toggling 'on' and 'off' the model give a good estimate of the silhouette line up, but does not help to compare plane changes of surfaces. This tool will help you do that. A 'good' line up is when it feels like the model is propagating along the surface of the reference. This is helpful for digital double work.

# What does it do ?
This tool allows the user to tweal the depth and opacity attributes of a given imagePlane. So it does nothing fancy, it is just a useful link. If the user has multiple viewports open to line up to different angles (i.e a setup with multiple cameras), the tool allows the user to use this "sliding" technique from one interface only, eliminating the needs of multiple Attribute Editor interfaces.
