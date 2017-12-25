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

![screenshot_20171225-114024](https://user-images.githubusercontent.com/454690/34342614-6d1b5904-e96a-11e7-9bca-d13e3ffc0135.png)

From the home screen, tap "Dashboard".

![screenshot_20171225-114045 1](https://user-images.githubusercontent.com/454690/34342702-dfcc8502-e96c-11e7-9ce3-a25856bd8ea3.png)

Tap in the big blank space to add elements to the dashboard.

![screenshot_20171225-114059 1](https://user-images.githubusercontent.com/454690/34342672-c3dd0552-e96b-11e7-8679-88516902d6ac.png)

Add "Position".

![screenshot_20171225-114200](https://user-images.githubusercontent.com/454690/34342676-ebfa06fc-e96b-11e7-89f3-b0e0abdd2fc6.png)

Tap on an empty space and also add "Accuracy":

![screenshot_20171225-114206](https://user-images.githubusercontent.com/454690/34342706-06f93d28-e96d-11e7-8677-c2943d92b0cd.png)

By default, these will show position English units and the minutes/seconds format of latitude and longitude.

In our work, we're using the Universal Trans-Mercator (UTM) coordinate system ([why? Here's a quick explainer.](https://www.maptools.com/tutorials/utm/why_use_utm))

Open the menu and go to Settings:

![screenshot_20171225-114324](https://user-images.githubusercontent.com/454690/34342713-4ed3db58-e96d-11e7-81cd-44923ae482dc.png)

In settings, select "Position Format".

![screenshot_20171225-114239](https://user-images.githubusercontent.com/454690/34342612-6ae215ec-e96a-11e7-9634-ce36708eb379.png)

In "Position Format", select "UTM".

![screenshot_20171225-114249](https://user-images.githubusercontent.com/454690/34342677-f68b73f8-e96b-11e7-9054-8883400f1cca.png)

Back in the Settings menu, select "Units".

![screenshot_20171225-114239](https://user-images.githubusercontent.com/454690/34342612-6ae215ec-e96a-11e7-9634-ce36708eb379.png)

Select Meters (standard for orienteering) so that you will see accuracy in meters.

![screenshot_20171225-114300](https://user-images.githubusercontent.com/454690/34342615-6e893612-e96a-11e7-8324-5a5240a6c238.png)

Get back to the dashboard by selecting "Standard" from the menu on the left:

![screenshot_20171225-114313 1](https://user-images.githubusercontent.com/454690/34342737-4f9b6a50-e96e-11e7-89e3-f4fe74bad4f4.png)

Here is our fully configured app, reporting out position coordinates in UTM and accuracy in meters:

![screenshot_20171225-114339](https://user-images.githubusercontent.com/454690/34342613-6bc905ec-e96a-11e7-8fa4-6f99d9b42986.png)
