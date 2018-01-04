# LiDAR Import

## Objective
Find and import LiDAR data into Open Orienteering Mapper to get contours using only free and open source tools.

Bonus points if it's GUI-only.

## Let's give it a shot.

### Where we're starting

The Puget Sound LiDAR Consortium is a publicly accessible repository for LiDAR scans of the Washington State Puget Sound area.

### Get a login
Web search for the Puget Sound LiDAR Consortium and follow the instructions to get a (free) username and password.

![screen shot 2018-01-03 at 3 27 20 pm](https://user-images.githubusercontent.com/454690/34548985-295da9e0-f0ba-11e7-9351-d27320ab54f0.png)

### Find the right data
[On the Data page of the Puget Sound LiDAR Consortium](http://pugetsoundlidar.ess.washington.edu/lidardata/restricted/PSLCbyproject.html) there's a list of different LiDAR projects by date, and a link to a map that helps you ID which projects include data for the area you're looking for.

The [map](https://www.arcgis.com/home/webmap/viewer.html?webmap=51796abb2ff8450f86a108ef6c8dce4f) (Project Viewer) lets you enter an address or place to zoom in on the correct area.

Searching for the area I'm mapping:

![screen shot 2018-01-03 at 3 35 45 pm](https://user-images.githubusercontent.com/454690/34548989-29bc90c2-f0ba-11e7-8b39-45e97aa232ec.png)

Gets us to this zoomed-in view and pop-up with details about the project:

![screen shot 2018-01-03 at 3 35 50 pm](https://user-images.githubusercontent.com/454690/34548988-299d7d40-f0ba-11e7-841a-b72dafacf74a.png)

Notice the (1 of 4) at the top! There are 4 projects that cover this area. We want the newest, probably? You can click through them here.

Back on the [Data page](http://pugetsoundlidar.ess.washington.edu/lidardata/restricted/PSLCbyproject.html) is a list of the projects.

I think I'd like to check out the [Snohomish River Estuary project](http://pugetsoundlidar.ess.washington.edu/lidardata/restricted/projects/2009snoho_river_est.html) from 2009:

![screen shot 2018-01-03 at 7 32 07 pm](https://user-images.githubusercontent.com/454690/34549346-d93f83fe-f0bc-11e7-94cf-76f8b157c572.png)

Looking more closely at the available data, I think we want the LAS files, which are raw LiDAR files.

![screen shot 2018-01-03 at 7 32 18 pm](https://user-images.githubusercontent.com/454690/34549345-d91e9fea-f0bc-11e7-91c2-60d685db37d3.png)

If we click through, we get this list of files:


![screen shot 2018-01-03 at 4 52 18 pm](https://user-images.githubusercontent.com/454690/34549366-0f5fdb1e-f0bd-11e7-834d-914022bf0b07.png)

Cool. Using the helpful `wget` command from the top of the page, I can download a bunch of .laz files, which I think include all the data I'll need.

For convenience, here's the command:

`wget -r -nH -np --http-user=myaccount --http-password=mypassword --cut-dirs=5 -nv http://pugetsoundlidar.org/lidardata/restricted/las/pslc2009/snohoriver/index.html`

(Don't forget to swap in your account name and password with the Puget Sound LiDAR Consortium!)

### File conversion, I assume
Ok, now I have a bunch of heavy .laz files. What do I do with these?

If I go into Open Orienteering Mapper, then File > Import, I can check what filetypes are permissible:

![screen shot 2018-01-03 at 7 37 16 pm](https://user-images.githubusercontent.com/454690/34549455-8f35afda-f0bd-11e7-86e6-5e5c471c69b2.png)

* .omap
* .xmap
* .ocd
* .shp
* .shx
* .gpx
* .osm
* .dxf

So if I can turn a .laz into one of those, I'm golden.

...What actually is a .laz file? According to a quick browse of the internet, it's a compressed .las file.

[ArcGIS has a nice article on what a .las is](http://desktop.arcgis.com/en/arcmap/10.3/manage-data/las-dataset/what-is-a-las-dataset-.htm). Worth a perusal– essentially, it's a point cloud.

I have a ton of files in my download from the Puget Sound LiDAR Consortium– I think each represents a relatively small geospatial area.

Somehow I stumbled across a link for this thing called [LAStools](http://www.cs.unc.edu/~isenburg/lastools/), which looks like it will come in handy for file conversion.
