# tif_to_gif

This code can be used to transform TIF files into animated GIF files. It mainly uses the tmap and gifski packages, but the function encoded here makes those functions more user friendly. This code makes it easier to select specific files in a folder of mixed files. It also allows for the user to generate more than one GIF at a time, so long as all the initial TIFF files are located in the same folder. 

### Script Files:

- `tif_to_gif.R` - This is a sourceable function to turn TIF files into GIF files. Call this .R file from a different file and provide the required inputs to use it. 
- `example_code.Rmd` - This is an example of how to source and use the function in tif_to_gif.R
- `example_without_fx.Rmd` - This is an example of how to use this code without using tif_to_gif.R. This is useful to have if you need to customize the process for a specific case. 

### Data Files:

- `adenfasc-X.tif` - 5 TIFF files as example data for the species Adenostoma fasciculatum
- `ceanramu-X.tif` - 5 TIFF files as example data for the species Ceanothus cuneatus var. fascicularis
- `landis_adenfasc.gif` - An example output, and placeholder to make sure the output_data folder exists

### Required/Recommended Packages:

- `tmap` - Required to make the animation
- `gifski` - Required for tmap, which is dependent on this package for creating GIFs
- `raster` - Required for the processing of raster data
- `gtools` - Required to import specific files (gtools::mixedsort)
- `here` - Useful for specifying file locations relative to Rproj
- `purrr` - Useful for running the function for more than one species/prefix at a time (purrr:pmap)

Author: Lauren Harris

With thanks to: Frank Davis
