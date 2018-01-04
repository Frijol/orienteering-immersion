# Georeferencing Points with Smartphone GPS

## Objective

Use a smartphone during fieldwork to find the positions of specific points (trail bends, intersections, rocks, man-made features, etc.) and map them in Open Orienteering Mapper.

## Materials

* An Android phone, or an iPhone and an app you personally know how to export waypoints from
* A laptop
* [Open Orienteering Mapper (0.7.0/Stable)](http://www.openorienteering.org/apps/mapper/): [Mac Download](https://github.com/OpenOrienteering/mapper/releases/download/v0.7.0/OpenOrienteering-Mapper-0.7.0-macOS.dmg) | [Windows Download](https://download.opensuse.org/repositories/home:/dg0yt/Windows/OpenOrienteering-Mapper_0.7.0-Windows-x64.exe)

## Instructions

## Waypoints
![0-1](https://user-images.githubusercontent.com/454690/34549670-4c241e6e-f0bf-11e7-82db-55ca54890857.png)
![0-4](https://user-images.githubusercontent.com/454690/34549671-4c41f826-f0bf-11e7-9019-d873e58c25a4.png)
![0-3](https://user-images.githubusercontent.com/454690/34549672-4c5b3890-f0bf-11e7-8c67-dce9dff27bc2.png)
![0-2](https://user-images.githubusercontent.com/454690/34549673-4c7869a6-f0bf-11e7-9f6d-e78cdf2d4266.png)
![0](https://user-images.githubusercontent.com/454690/34549674-4d158fa6-f0bf-11e7-8304-cbbdf96ae0de.png)


## Importing waypoints into open orienteering mapper

In Open Orienteering Mapper, go to File > Import, and find your exported waypoints.

If you're using the GPS Essentials Android app, it will probably be called something like "Waypoints.kml".

By default, your .kml file will be grayed out (not selectable). This is because in theory, a .kml is not an importable filetype.

But, I did it anyway, and it worked (*shrug*). Go ahead and click the little dropdown at the bottom of the Open File dialog and switch the selection from "Importable files..." to "All files".

(This image shows the theoretically acceptable file types to import:)

![screen shot 2018-01-03 at 7 37 16 pm](https://user-images.githubusercontent.com/454690/34549455-8f35afda-f0bd-11e7-86e6-5e5c471c69b2.png)

(Note the "All files" selection below.)

![screen shot 2018-01-03 at 8 23 48 pm](https://user-images.githubusercontent.com/454690/34550302-93ac7678-f0c4-11e7-9b97-0ece8a1ce315.png)

Open your file to import.

Cool, a bunch of pink dots!

![screen shot 2018-01-03 at 8 24 33 pm](https://user-images.githubusercontent.com/454690/34550301-9396573a-f0c4-11e7-80ff-0d353543655c.png)

I have my imported waypoints superimposed on a Runkeeper template of the trails, for reference.

## Turning waypoints into map features

Because these waypoints were imported directly (rather than as a template), you can directly convert them into features on the map.

Start with a small group of pink dots that are all destined to become the same symbol (or, just pick one pink dot).

Select the items you would like to convert into map symbols with the white arrow "Edit object" tool.

![screen shot 2018-01-03 at 8 33 10 pm](https://user-images.githubusercontent.com/454690/34550394-6aebb432-f0c5-11e7-8a27-0c3729812ce0.png)

Select the symbol you'd like to convert your points to (in my case, the green X "Special vegetation feature" because I overzealously mapped individual trees).

![screen shot 2018-01-03 at 8 33 17 pm](https://user-images.githubusercontent.com/454690/34550397-6b3c44f6-f0c5-11e7-8a91-8c1d6394118d.png)

Click the "Switch symbol" button.

![screen shot 2018-01-03 at 8 32 22 pm](https://user-images.githubusercontent.com/454690/34550393-6ad026b8-f0c5-11e7-8719-28e2fd3964da.png)

*The correct button is the black box and arrow, **not** the yellow circle (that is a fill symbol which will superimpose your symbol and the original weird imported symbol– so if you're getting doubled symbols, that's where you went wrong).*

Hey presto! The selected points are now green X tree symbols instead of pink dots.

![screen shot 2018-01-03 at 8 33 29 pm](https://user-images.githubusercontent.com/454690/34550396-6b1e158a-f0c5-11e7-8e62-f0421a54b003.png)

Repeat as necessary...

![screen shot 2018-01-03 at 8 32 57 pm](https://user-images.githubusercontent.com/454690/34550395-6b03975a-f0c5-11e7-9745-a5db1a80df44.png)
