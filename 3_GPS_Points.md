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


![screen shot 2018-01-03 at 7 54 42 pm](https://user-images.githubusercontent.com/454690/34550215-da92492e-f0c3-11e7-98c9-190d02e9d21d.png)
![screen shot 2018-01-03 at 7 54 07 pm](https://user-images.githubusercontent.com/454690/34550216-daabcd40-f0c3-11e7-9186-505aa0e9a5ba.png)
![screen shot 2018-01-03 at 7 54 27 pm](https://user-images.githubusercontent.com/454690/34550217-dac432d6-f0c3-11e7-9864-208726993895.png)
![screen shot 2018-01-03 at 7 54 18 pm](https://user-images.githubusercontent.com/454690/34550218-dadd4118-f0c3-11e7-8e29-d2b6c1074e17.png)
![screen shot 2018-01-03 at 7 54 49 pm](https://user-images.githubusercontent.com/454690/34550219-db197fa2-f0c3-11e7-97e7-a181f6ce9edb.png)
![screen shot 2018-01-03 at 7 54 34 pm](https://user-images.githubusercontent.com/454690/34550220-db44e020-f0c3-11e7-99b2-c901eeb7c7d6.png)
![screen shot 2018-01-03 at 7 57 23 pm](https://user-images.githubusercontent.com/454690/34550221-db8c8006-f0c3-11e7-84be-974ad4bd6c0b.png)
