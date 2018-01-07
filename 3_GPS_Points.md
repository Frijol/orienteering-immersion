# Georeferencing Points with Smartphone GPS

## Objective

Use a smartphone during fieldwork to find the positions of specific points (trail bends, intersections, rocks, man-made features, etc.) and map them in Open Orienteering Mapper.

## Materials

* An Android phone, or an iPhone and an app you personally know how to export waypoints from
* A laptop
* [Open Orienteering Mapper (0.7.0/Stable)](http://www.openorienteering.org/apps/mapper/): [Mac Download](https://github.com/OpenOrienteering/mapper/releases/download/v0.7.0/OpenOrienteering-Mapper-0.7.0-macOS.dmg) | [Windows Download](https://download.opensuse.org/repositories/home:/dg0yt/Windows/OpenOrienteering-Mapper_0.7.0-Windows-x64.exe)

## Instructions

### Collect Waypoints
Let's get out into the field! With the GPS Essentials app downloaded, go someplace with features you want to map.

From the home screen of the GPS Essentials app, go to Waypoints (the pushpin on the right):

<img src="https://user-images.githubusercontent.com/454690/34549674-4d158fa6-f0bf-11e7-8304-cbbdf96ae0de.png" width="250">

Press the "+" button in the lower right to make a waypoint.

<img src="https://user-images.githubusercontent.com/454690/34549670-4c241e6e-f0bf-11e7-82db-55ca54890857.png" width="250">

Below is the waypoint creation screen.

Notice the detail shown of "20 satellites visible..."– that number at the end is the potential for error, and you want it as low as possible (4.55m is good).

You can pick a symbol, and optionally name the point (mine is a rootstock), then press Create.

<img src="https://user-images.githubusercontent.com/454690/34549671-4c41f826-f0bf-11e7-9019-d873e58c25a4.png" width="250">

The GPS Essentials app gives us a number of symbols we can use to record points.

As a mapper, it's your choice which symbols to use/whether to name waypoints/etc. Just make sure you figure out a system where you'll remember what you were noting when you get back to the computer!

Here are some of the available symbols:

<img src="https://user-images.githubusercontent.com/454690/34549673-4c7869a6-f0bf-11e7-9f6d-e78cdf2d4266.png" width="250">

You can use waypoints to get any kind of reference point, not just point features! Here I'm noting the position of a change in vegetation:

<img src="https://user-images.githubusercontent.com/454690/34549672-4c5b3890-f0bf-11e7-8c67-dce9dff27bc2.png" width="250">

Here is a list of waypoints I took while out mapping– notice that I've used different symbols and named some of the waypoints. This will make it easier for me to know what symbols to use for these points later.

<img src="https://user-images.githubusercontent.com/454690/34549670-4c241e6e-f0bf-11e7-82db-55ca54890857.png" width="250">

Once you've collected a few points, head back inside to put them on your map.

## Export waypoints and send them to yourself

On your phone, you should still be in the Waypoints section of GPS Essentials.

Tap on the menu icon in the top right, then select Export.

<img src="https://user-images.githubusercontent.com/454690/34645085-8f1f98c4-f2f9-11e7-8f96-6ac299098516.png" width="250">

Swipe through the icons shown below SHARE until you find one you can use to send the file to yourself (I used an email app):

<img src="https://user-images.githubusercontent.com/454690/34645083-8ef5b16c-f2f9-11e7-9785-311f1c612ac3.png" width="250">

## Set up your Open Orienteering Mapper file

On your computer, open Open Orienteering Mapper ("Mapper").

Ideally, you would do this with a map you already have some information about– e.g. do the [Mapping Trails with Runkeeper](/1_Runkeeper_Trails.html) tutorial before this one, or [bring in a template from Open Street Map](1.1_Runkeeper_OSM.html) if you don't want to go back outside right now.

Otherwise, you're mapping points into empty space, which can be confusing.

## Import waypoints into open orienteering mapper

In Open Orienteering Mapper, go to File > Import, and find the waypoints you exported from your app (I emailed them to myself and then downloaded to my computer).

If you're using the GPS Essentials Android app, the file will probably be called something like "Waypoints.kml".

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

## Turn waypoints into map features

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

## How do I know which pink dots are what?

If you took a lot of waypoints (like I did), you might not remember what they all are when you get back to the computer.

But of course you took notes in the app while you were doing fieldwork!

Put your phone next to your computer; you'll be looking back and forth between the two screens a lot.

Tap on the map in Waypoints:

<img src="https://user-images.githubusercontent.com/454690/34645080-8eb9fc3a-f2f9-11e7-8ead-86912e96097e.png" width="250">

Turn your phone so its orientation matches up with the map of dots on your computer.

You can pinch to zoom in and get a clearer picture of your symbols:

<img src="https://user-images.githubusercontent.com/454690/34645081-8ecdb040-f2f9-11e7-81e6-dbbca04fcd36.png" width="250">

You can tap on points in order to see their names. Tap on the name bubbles to close them again.

<img src="https://user-images.githubusercontent.com/454690/34645084-8f09b5b8-f2f9-11e7-9416-46ff79de7a24.png" width="250">

After ~half an hour of converting my GPS points into the symbols they represent, here is my map (still overlaid on a Runkeeper trace of the trails):

![screen shot 2018-01-04 at 12 24 08 pm](https://user-images.githubusercontent.com/454690/34645079-8ea5c24c-f2f9-11e7-8d9a-2d2092593c27.png)
