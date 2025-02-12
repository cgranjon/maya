# Main Command (MEL)
cg_transfer();

# How to install
Save the script in your "../maya/../scripts/" directory.

# How to use
This tool is mainly designed to batch transfer data between models via ordered lists of polygonal objects.

The tool works in two different ways:
- 1 source object and multiple targets
- an equal number of sources and targets

For now there is only a limited number of options to choose from:
- "Marvelous Designer": Once you have similated cloth with Marvelous Designer, export the sim mesh and the garments mesh. In Maya retopo the garment and follow the tooltip of the checkbox.
- "UVs": Transfers UVs  between the ordered lists. Only one configuration is available at the moment (Transfers the 'current' UVset, Sample space = Component).
- "Vertices Position from UVs": As the name suggests, transfer vertex position looking at the UVmap.
- "Blendshape": Adds a blendShape node to the target objects. The 'source' objects are the weights targets. Sets the weights to 1 by default.
- "Blendshape with deltas": Adds a blendShape node to the target objects. Sets the weights to 1 by default. The 'source' and 'other' objects are the weights targets. The 'other' object are considered "offsets".
- "Transform Values": Transfers the transform values of the 'source' objects to the 'target' objects. It captures the worldd-space transform values of the 'source' objects, so it works even if the 'source' objects are nested in groups.

# Notes


# Why this tool ?


# What does it do ?

