# Landsat C2 Stack Pulls

These scripts function as the primary R-user-friendly version of the Landsat Collection 2 workflows for the ROSS lab. These files are meant to function as building blocks, where you can use some or all to create a dataset.

This iteration is for the Sky and Loch Ponds for a bit of exploration into the ARP product and the differences between ARP and C2 data.

## Folder/file descriptions:

* literateCode:

These are the primay working scripts of this subdirectory. The scripts in this folder are considered 'literate code', meaning they are end-user friendly with lots of commenting and have a lot of code chunks to run. The `pySetup.R` is code that is sourced in the other scripts, and these scripts can be run in any order. This code only has to be run once and the output goes to the user's Drive folder. The scripts in the path `sky-loch-explore/programs` collate the data created in these scripts and also copy the data to a local OneDrive folder, connected in the subdirectory `sky-loch-explore/data`.

    -  LandsatC2_M4-7_SurfaceRefTempStacks.rmd: level 2 surface reflectance and surface temperature stack pull for Landsat Collection 2 missions 4-7

    -  LandsatC2_M8-9_SurfaceRefTempStacks.rmd: level 2 surface reflectance and surface temperature stack pull for Landsat Collection 2 missions 8 and 9

    -  LandsatC2_M8-9_L1_ProvisionalSceneList.Rmd: this script grabs the necessary metadata to place an order for the Provisional Landsat Aquatic Reflectance Product

    -   pySetup.R: script that uses the `reticulate` package to set up a reproducible python environement compatible with R
 