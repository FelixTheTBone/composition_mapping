# Composition mapping script
## Overview
This repository provides a simple python script to plot compositional 2D maps obtained, e.g. from EDXS or EPMA. 
It is far from perfect, so please use responsibly. I will try and make improvements with time, and see it as a small project to improve and learn.
I have been using it predominantly with Linux but it should be quite platform agnostic.

Feel free to let me know any potential improvements or bugs that need figuring out, cheers. 


## Calculations
All data is mapped directly and therefore requires x-y-matrices, see input & export.
To improve the contrast across maps, each map is individually normalized. Please mind, that this applies to (semi-)quantitative EDXS or EMPA maps.
For quantitative maps, the normalization step should be skipped and units printed printed in the colorbar appropriately.

The normalization step sets the map minimum $v_{min} = 0$ and sets the displayed maximum to $v_{max} = 0.1 \cdot Map_{max}$.
Here $Map_{max}$ refers to the maximum of the map overall, which can be noise or some strong local segregation.


## Example data
The folder 'input' contains a set of example data. In its current format the script is adding a scale bar in the first map only.
Here is an example of the Al map, acknowledgements to matplotlib-scalebar.

![Al composition map of example data (export).](https://github.com/FelixTheTBone/composition_mapping/blob/main/export/Al%20K%20series.png)

The following maps will be plotted without scalebar, in most use cases it would be unnecessary to have it in each map.
Here are two examples of a Ni map and a Nb map, respectively.

![Ni composition map of example data (export).](https://github.com/FelixTheTBone/composition_mapping/blob/main/export/Ni%20L%20series.png)
![Nb composition map of example data (export).](https://github.com/FelixTheTBone/composition_mapping/blob/main/export/Nb%20L%20series.png)


## Input & export


## Citing

