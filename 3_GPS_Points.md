# Georeferencing Points with Smartphone GPS

## Objective

Use a smartphone during fieldwork to find the positions of specific points (trail bends, intersections, rocks, man-made features, etc.) and map them in Open Orienteering Mapper.

## Materials

* An Android phone, or an iPhone and an app you yourself configure to show you UTM coordinates
* A laptop
* [Open Orienteering Mapper (0.7.0/Stable)](http://www.openorienteering.org/apps/mapper/): [Mac Download](https://github.com/OpenOrienteering/mapper/releases/download/v0.7.0/OpenOrienteering-Mapper-0.7.0-macOS.dmg) | [Windows Download](https://download.opensuse.org/repositories/home:/dg0yt/Windows/OpenOrienteering-Mapper_0.7.0-Windows-x64.exe)

## Instructions
### Configure app

You will need to set up your smartphone to tell you:

1. Your GPS coordinates, in UTM format
1. The accuracy of the coordinates reported

If you have an Android, great! Continue for detailed instructions using the app GPS Essentials.

If you have an iPhone, sorry, I don't... so you will have to figure this part out yourself. Internet research tells me that [Polaris](http://appcrawlr.com/android/polaris-navigation-system) might be a good free app for this, but I haven't tried it.

#### Setting up GPS Essentials for Android

Download the app [GPS Essentials](https://play.google.com/store/apps/details?id=com.mictale.gpsessentials&hl=en) and open it.

The app will immediately ask you if it can access location. Click "Allow".

<img src="https://user-images.githubusercontent.com/454690/34342614-6d1b5904-e96a-11e7-9bca-d13e3ffc0135.png" width="250">

From the home screen, tap "Dashboard".

<img src="https://user-images.githubusercontent.com/454690/34342702-dfcc8502-e96c-11e7-9ce3-a25856bd8ea3.png" width="250">

Tap in the big blank space to add elements to the dashboard.

<img src="https://user-images.githubusercontent.com/454690/34342702-dfcc8502-e96c-11e7-9ce3-a25856bd8ea3.png" width="250">

Add "Position".

<img src="https://user-images.githubusercontent.com/454690/34342676-ebfa06fc-e96b-11e7-89f3-b0e0abdd2fc6.png" width="250">

Tap on an empty space and also add "Accuracy":

<img src="https://user-images.githubusercontent.com/454690/34342706-06f93d28-e96d-11e7-8677-c2943d92b0cd.png" width="250">

By default, these will show position English units and the minutes/seconds format of latitude and longitude.

In our work, we're using the Universal Trans-Mercator (UTM) coordinate system ([why? Here's a quick explainer.](https://www.maptools.com/tutorials/utm/why_use_utm))

Open the menu and go to Settings:

<img src="https://user-images.githubusercontent.com/454690/34342713-4ed3db58-e96d-11e7-81cd-44923ae482dc.png" width="250">

In settings, select "Position Format".

<img src="https://user-images.githubusercontent.com/454690/34342612-6ae215ec-e96a-11e7-9634-ce36708eb379.png" width="250">

In "Position Format", select "UTM".

<img src="https://user-images.githubusercontent.com/454690/34342677-f68b73f8-e96b-11e7-9054-8883400f1cca.png" width="250">

Back in the Settings menu, select "Units".

<img src="https://user-images.githubusercontent.com/454690/34342612-6ae215ec-e96a-11e7-9634-ce36708eb379.png" width="250">

Select Meters (standard for orienteering) so that you will see accuracy in meters.

<img src="https://user-images.githubusercontent.com/454690/34342615-6e893612-e96a-11e7-8324-5a5240a6c238.png" width="250">

Get back to the dashboard by selecting "Standard" from the menu on the left:

<img src="https://user-images.githubusercontent.com/454690/34342737-4f9b6a50-e96e-11e7-89e3-f4fe74bad4f4.png" width="250">

Here is our fully configured app, reporting out position coordinates in UTM and accuracy in meters:

<img src="https://user-images.githubusercontent.com/454690/34342613-6bc905ec-e96a-11e7-8fa4-6f99d9b42986.png" width="250">


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
