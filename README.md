# tif_to_gif

This code can be used to transform TIFF files into animated GIF files. It uses the tmap and gifski packages, but the function encoded here makes those functions more user friendly. This code makes it easier to select specific files in a folder of mixed files. It also allows for the user to generate more than one GIF at a time, so long as all the initial TIFF files are located in the same folder. 

### Script Files:

- **tif_to_gif.R** - This is a sourceable function to turn TIF files into GIF files. Call this .R file from a different file and provide the required inputs to use it. 
- **example_code.Rmd** - This is an example of how to source and use the function in tif_to_gif.R
- **example_without_fx.Rmd** - This is an example of how to use this code without using tif_to_gif.R. This is useful to have if you need to customize the process for a specific case. 

### Data Files:

- **adenfasc-X.tif** - 5 TIFF files as example data for the species Adenostoma fasciculatum
- **ceanramu-x.tif** - 5 TIFF files as example data for the species Ceanothus cuneatus var. fascicularis