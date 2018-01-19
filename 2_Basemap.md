# Building a Basemap from Screen Captures

## Objective

Find useful map data from the internet (such as satellite imagery, street map data, and contours), import it with georeferencing into an Open Orienteering Mapper file, and trace it to make a no-fieldwork map.

Example result:

![screen shot 2018-01-19 at 1 44 32 pm](https://user-images.githubusercontent.com/454690/35173071-e93045d2-fd1e-11e7-9640-c394582dc5e6.png)

---
### Theory & philosophy– side note for the curious

*Ideally, we would source up-to-date images that come with georeferencing data built in, such that we don't have to do any manual (and potentially wonky) template adjustment in Open Orienteering Mapper. I don't know yet if this is possible.*

*In the meanwhile, the approach is to (1) get some data from Open Street Map– not as much detail as a satellite image, but correctly georeferenced, then (2) pull satellite images for which we know the scale in meters per pixel, if not the exact positioning, then drag them visually into alignment with the georeferenced data.*

*What I'm presenting here is a functional and expedient approach. It works. I'd rather do it differently. I'm working in the "[sat](https://github.com/Frijol/orienteering-immersion/tree/sat)" branch of this repository on this problem if you want to track my progress.*

---

## Materials

* A computer
* [Open Orienteering Mapper (0.7.0/Stable)](http://www.openorienteering.org/apps/mapper/): [Mac Download](https://github.com/OpenOrienteering/mapper/releases/download/v0.7.0/OpenOrienteering-Mapper-0.7.0-macOS.dmg) | [Windows Download](https://download.opensuse.org/repositories/home:/dg0yt/Windows/OpenOrienteering-Mapper_0.7.0-Windows-x64.exe)
* The ability to take screen shots (screen captures). If this is new to you, try everything in [this LifeHacker article](https://lifehacker.com/5825771/how-to-take-a-screenshot-or-picture-of-whats-on-your-computer-screen) that applies to your computer (Windows/Mac) before proceeding.

## Instructions

### Get georeferenced

Choose an area to map, such as your house or a park. In this example, I'm mapping Brightwater Treatment Plant, which is a nice park in addition to being a water treatment plant.

Go to [Open Street Map](http://www.openstreetmap.org/) and search for your location.

![screen shot 2018-01-19 at 12 09 42 pm](https://user-images.githubusercontent.com/454690/35169594-f4bdd732-fd11-11e7-8f48-fab087ae7fe4.png)

Once you have the area you want to map on your screen, click the Export button near the top left of the page.

![screen shot 2018-01-19 at 12 10 37 pm](https://user-images.githubusercontent.com/454690/35169595-f4d1422c-fd11-11e7-9665-819b4f6355c9.png)

Click Export to download a file with data about the area (likely called something like "map.osm").

![screen shot 2018-01-19 at 12 11 04 pm](https://user-images.githubusercontent.com/454690/35169593-f4a9e74a-fd11-11e7-86f1-6b696e88d0b9.png)

Leave the Open Street Maps page open on your computer; we're going to use it again later.

Now open Open Orienteering Mapper on your computer. Click "Create a new map..."

![screen shot 2018-01-19 at 12 14 47 pm](https://user-images.githubusercontent.com/454690/35169786-bbb9a9d8-fd12-11e7-80b0-866e420ef875.png)

I've decided to make a sprint map, so I change the scale to 1:5000 and select the symbol set "ISSOM_5000" before clicking "Create".

![screen shot 2018-01-19 at 12 15 00 pm](https://user-images.githubusercontent.com/454690/35169787-bbd4e888-fd12-11e7-859e-45229610a660.png)

Here is our new, blank map file:

![screen shot 2018-01-19 at 12 15 10 pm](https://user-images.githubusercontent.com/454690/35169784-bb7f03a0-fd12-11e7-8e03-3cd3933aadd1.png)

Go to Templates > Open template...

![screen shot 2018-01-19 at 12 15 27 pm](https://user-images.githubusercontent.com/454690/35169789-bc163e6e-fd12-11e7-9b51-85f85349ade2.png)

Find the .osm file you just exported from Open Street Maps.

Once you click Open, it will ask you if you want your track georeferenced or not. You do!

Select "Georeferenced".

![screen shot 2018-01-19 at 12 16 39 pm](https://user-images.githubusercontent.com/454690/35169790-bc620c40-fd12-11e7-88d0-a728ebee8ee0.png)

In order to georeference the template to the map, Open Orienteering Mapper needs to know how we want to georeference our map. It pops up this screen:

![screen shot 2018-01-19 at 12 16 47 pm](https://user-images.githubusercontent.com/454690/35169788-bbf8ab24-fd12-11e7-9653-923cae0ae6c3.png)

Click on the drop-down box next to "Coordinate reference system" and select UTM to choose the Universal Trans-Mercator coordinate system.

![screen shot 2018-01-19 at 12 16 54 pm](https://user-images.githubusercontent.com/454690/35169791-bc821576-fd12-11e7-91bc-9fea760b1797.png)

Here is our map, now with a georeferenced template:

![screen shot 2018-01-19 at 12 17 04 pm](https://user-images.githubusercontent.com/454690/35169785-bb9a2c70-fd12-11e7-9198-80af2e0c0cb3.png)

It's important to start with georeferenced data so that we can use the other, GPS-based mapping techniques in this tutorial (e.g. the Runkeeper Trail Mapping) and have everything show up in correct positions.

We are going to use this Open Street Map data as a reference to line up other, more detailed images as templates to trace.

### Get satellite imagery
We are going to use a free tool called [GeoLocator](http://tools.freeside.sk/geolocator/geolocator.html), because it tells us scale in pixels per meter (this will come in handy soon).

Open [GeoLocator](http://tools.freeside.sk/geolocator/geolocator.html).

![screen shot 2018-01-19 at 12 39 29 pm](https://user-images.githubusercontent.com/454690/35170768-2cdff7ea-fd16-11e7-98c7-ad65bbee42d6.png)

Wow, the whole world! GeoLocator wants coordinates in order to find your location.

Tab back over to the Open Street Map page we used earlier.

At the end of the URL, you will see the coordinates of your map!

![screen shot 2018-01-19 at 12 08 21 pm](https://user-images.githubusercontent.com/454690/35169596-f4fe49d4-fd11-11e7-803b-eeb8fb8739d8.png)

Copy the coordinates from the URL, tab back over to the GeoLocator page, and paste them into the coordinates box:

![screen shot 2018-01-19 at 12 41 13 pm](https://user-images.githubusercontent.com/454690/35170766-2cabf8c8-fd16-11e7-9d61-fa139478259b.png)

Press "Apply" to see your location centered and marked on the map.

![screen shot 2018-01-19 at 12 41 35 pm](https://user-images.githubusercontent.com/454690/35170769-2cf93818-fd16-11e7-84de-70a22b5374cb.png)

Zoom in until you have a useful area centered on the screen:

![screen shot 2018-01-19 at 12 42 06 pm](https://user-images.githubusercontent.com/454690/35170767-2cc7a316-fd16-11e7-8c65-ff0ab6dac958.png)

Now take a screen shot, being sure to capture the part in the bottom right where it says "1px = ...":

![screen shot 2018-01-19 at 12 44 30 pm](https://user-images.githubusercontent.com/454690/35170881-8da736c4-fd16-11e7-896f-6ea56e0566bc.png)

Make sure you know the file location where the screen shot is saved.

### Import imagery into Open Orienteering Mapper

In Open Orienteering Mapper, go to Templates > Open template...

![screen shot 2018-01-19 at 12 15 27 pm](https://user-images.githubusercontent.com/454690/35169789-bc163e6e-fd12-11e7-9b51-85f85349ade2.png)

Find your screen shot and click "Open".

It will ask for scaling information. We know how many meters per pixel! In my case, 1px - 3.2x3.2m, so I enter 3.2:

![screen shot 2018-01-19 at 12 48 36 pm](https://user-images.githubusercontent.com/454690/35171017-18c5b88e-fd17-11e7-8dad-2db618ff0750.png)

When I press "Open", I now have my two templates on top of each other, like so:

![screen shot 2018-01-19 at 12 49 14 pm](https://user-images.githubusercontent.com/454690/35171032-2d01ab78-fd17-11e7-960f-7000faa0c80e.png)

### Working with multiple templates

This seems like a good moment to point you to the [Open Orienteering Mapper Manual page on Templates](http://www.openorienteering.org/mapper-manual/pages/templates-index.html). If you get lost in this tutorial, have a look at the manual page for more information.

Looking at your map, you may notice two issues immediately:

1. One template is blocking the other
1. The two templates don't line up correctly

We can fix that! All of the tools we need are in the Template Setup Window, which is probably already open.

If you're not sure if it's open, make sure there's a check mark in the Templates menu like so:

![screen shot 2018-01-19 at 12 52 10 pm](https://user-images.githubusercontent.com/454690/35171157-9464743a-fd17-11e7-8efa-4deb40abf40c.png)

#### Manipulating template settings

This section fixes the problem of templates blocking each other.

---

##### Adjusting template transparency

I'd like to be able to see through my satellite image to the Open Street Map data below. Let's adjust transparency.

In the template window, I know that the satellite image is the one called Screen Shot:

![screen shot 2018-01-19 at 12 53 53 pm](https://user-images.githubusercontent.com/454690/35171229-df16d8d8-fd17-11e7-9275-53e0fe2fc44e.png)

Click on the "100%" number under the "Opacity" column. Type "60" to get 60% opacity.

![screen shot 2018-01-19 at 12 54 01 pm](https://user-images.githubusercontent.com/454690/35171228-def70f62-fd17-11e7-9c4c-343235e17eff.png)

See the result:

![screen shot 2018-01-19 at 12 54 06 pm](https://user-images.githubusercontent.com/454690/35171227-dedca4ba-fd17-11e7-9f7b-696912008d4e.png)

##### Hiding and showing Templates

Maybe I don't want to see my satellite image at all right now.

Uncheck the checkbox next to the satellite image template file:

![screen shot 2018-01-19 at 12 57 57 pm](https://user-images.githubusercontent.com/454690/35171368-77411952-fd18-11e7-90bb-b0709f04dcd7.png)

It's gone!

![screen shot 2018-01-19 at 12 58 02 pm](https://user-images.githubusercontent.com/454690/35171367-77297158-fd18-11e7-8b6e-be19623576e3.png)

Ok, re-check that box. We need that template visible.

##### Changing template order

I'm finding it a little hard to make out the lines of the street map data through the semi-opaque satellite image:

![screen shot 2018-01-19 at 1 00 25 pm](https://user-images.githubusercontent.com/454690/35171509-defc6812-fd18-11e7-9977-9510fdd3c7c0.png)

I'd prefer to have the street map data show on top of the satellite image.

Select the open street map file (.osm) in the template list:

![screen shot 2018-01-19 at 1 00 50 pm](https://user-images.githubusercontent.com/454690/35171514-df3d622c-fd18-11e7-9e11-75dd07bc660c.png)

Click the little green up-arrow at the bottom of the Templates window to change the order of the template layers:

![screen shot 2018-01-19 at 1 00 56 pm](https://user-images.githubusercontent.com/454690/35171512-df0e985c-fd18-11e7-8dea-abf2c6cf33f5.png)

See that the .osm layer is now listed above the screen shot layer:

![screen shot 2018-01-19 at 1 04 04 pm](https://user-images.githubusercontent.com/454690/35171610-42c08aa4-fd19-11e7-957a-c7d63b4cc988.png)

Now the pink lines are on top of the satellite image:

![screen shot 2018-01-19 at 1 01 09 pm](https://user-images.githubusercontent.com/454690/35171513-df269786-fd18-11e7-9bf8-2bc5c03ac030.png)

It's still a bit hard to see, I think.

Adjust however you need to in order to see your data clearly.

Here, I've adjusted the satellite image template back to 100% opacity, but now the street map data is on top:

![screen shot 2018-01-19 at 1 01 19 pm](https://user-images.githubusercontent.com/454690/35171508-dee567ac-fd18-11e7-9596-6b5d1e0677aa.png)

Here is how I left my templates:

![screen shot 2018-01-19 at 1 03 46 pm](https://user-images.githubusercontent.com/454690/35171613-42d88cee-fd19-11e7-8ce6-2e3d46865cb7.png)

---

#### Positioning the satellite image

Recall that our Open Street Map data is georeferenced and that our screen shot satellite imagery is not.

This means that since our two templates are not lining up, the .osm layer is correctly positioned, and the screen shot layer needs to be adjusted to match.

We are going to do this visually. Use any distinctive shapes on your templates to find a point that should be the same in both places.

In your Templates window, select the Screen Shot layer:

![screen shot 2018-01-19 at 1 16 20 pm](https://user-images.githubusercontent.com/454690/35172082-1793ac74-fd1b-11e7-9320-68ac4e1effb6.png)

Click the little blue Move symbol at the bottom of the Templates window:

![screen shot 2018-01-19 at 1 16 25 pm](https://user-images.githubusercontent.com/454690/35172084-17c5f6e8-fd1b-11e7-9397-db1c76084c81.png)

You can now drag your satellite image into alignment with the open street map data. Zoom in as needed to make sure you are in as tight of alignment as you can manage:

![screen shot 2018-01-19 at 1 17 09 pm](https://user-images.githubusercontent.com/454690/35172083-17aaee0c-fd1b-11e7-80f2-7941e5f841f7.png)

Deselect the Move symbol ![screen shot 2018-01-19 at 1 16 25 pm](https://user-images.githubusercontent.com/454690/35172084-17c5f6e8-fd1b-11e7-9397-db1c76084c81.png) so that you don't move the template again by accident.

### Trace from the templates

Now that your templates are correctly positioned, you can use them to draw features!

It may be helpful to use the Templates window to give your Map layer some transparency.

Here's what a map-in-progress might look like:

![screen shot 2018-01-19 at 1 43 43 pm](https://user-images.githubusercontent.com/454690/35173043-cfffdffa-fd1e-11e7-8651-093d5a702771.png)

And here is the same map, with no templates and map transparency at 100%:

![screen shot 2018-01-19 at 1 44 32 pm](https://user-images.githubusercontent.com/454690/35173071-e93045d2-fd1e-11e7-9640-c394582dc5e6.png)
