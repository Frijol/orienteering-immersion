# Trail Mapping with RunKeeper

## Objective

Create a georeferenced trail map in Open Orienteering Mapper using Runkeeper to collect path data.

Example result:

![screen shot 2018-01-06 at 4 54 08 pm](https://user-images.githubusercontent.com/454690/34645437-437dc63a-f302-11e7-9928-e58ad34c6da8.png)

## Materials

### Physical materials
* A computer
* A smartphone

### Software downloads (free)
* [Runkeeper](https://runkeeper.com/): [Android Download](https://play.google.com/store/apps/details?id=com.fitnesskeeper.runkeeper.pro) | [iPhone Download](https://itunes.apple.com/us/app/id300235330?mt=8)
* [Open Orienteering Mapper (0.7.0/Stable)](http://www.openorienteering.org/apps/mapper/): [Mac Download](https://github.com/OpenOrienteering/mapper/releases/download/v0.7.0/OpenOrienteering-Mapper-0.7.0-macOS.dmg) | [Windows Download](https://download.opensuse.org/repositories/home:/dg0yt/Windows/OpenOrienteering-Mapper_0.7.0-Windows-x64.exe)

### Reference
* [The Open Orienteering Mapper Manual](http://www.openorienteering.org/mapper-manual/pages/)

## Instructions

### Get out on the trails

[Log in](https://support.runkeeper.com/hc/en-us/articles/201109446-How-do-I-get-started-with-the-RunKeeper-App-on-my-iPhone-) and [start a workout](https://blog.runkeeper.com/8/the-beginners-guide-to-tracking-your-first-workout-in-runkeeper/) such as a walk or run in Runkeeper. (Links here are tutorials on the Runkeeper blog.) Make sure your GPS is enabled and your timer is counting.

Walk or run trails!

### Get your GPS trail onto your computer

Conclude your workout in Runkeeper, then use the share button to send the workout link to yourself (for access from your computer).

![unnamed](https://user-images.githubusercontent.com/454690/34329289-899443e0-e8af-11e7-8b46-118180ddff7e.png)

(Within "Share", make sure you're on the "Map" tab in order to see the share button.)

This is the email the app sent to me through the "share" function:

![screen shot 2017-12-24 at 1 38 16 pm](https://user-images.githubusercontent.com/454690/34329324-aabf3f7e-e8b0-11e7-83da-813b1bae73f7.png)

Click the link (you'll have to log in) to see your activity on your computer:

![screen shot 2017-12-24 at 1 49 38 pm](https://user-images.githubusercontent.com/454690/34329352-5125d7b0-e8b1-11e7-9686-cea7eb16ea33.png)

Scroll down to the bottom of this page and click "GPX" under the "Export" section:

![screen shot 2017-12-24 at 1 50 57 pm](https://user-images.githubusercontent.com/454690/34329360-cc3eaad0-e8b1-11e7-9ac1-3fc1e4f506f2.png)

This will download a .gpx file of the route you walked/ran.

### Create a new map in Open Orienteering Mapper

*If you already did the Face Mapping exercise, this will be very familiar.*

Click "Create a new map..." in the upper left under **Activities**.

![screen shot 2017-12-22 at 11 44 52 am](https://user-images.githubusercontent.com/454690/34310655-9a84f5ee-e70d-11e7-9129-9a9ce8e2e8da.png)

Leave the default scale of 1:10000, but **–important!–** change the Symbol Set to "**ISOM2000_10000**". Then click **Create**.

![screen shot 2017-12-22 at 1 49 51 pm](https://user-images.githubusercontent.com/454690/34313308-0c05ae3c-e71f-11e7-9874-183c244fa8e9.png)

Tada! Now you have a brand new mapping canvas to work with.

![screen shot 2017-12-24 at 12 04 57 pm](https://user-images.githubusercontent.com/454690/34328916-b3a37118-e8a2-11e7-8b96-ef607ab21981.png)

### Set up georeferencing in your map

Here, we're going to tell Open Orienteering Mapper that we're using UTM coordinates (a format of latitude and longitude) so that any GPS coordinates we take in the field will show up in the right place on the map.

In the "Map" menu, select "Georeferencing..."

![screen shot 2017-12-24 at 2 05 20 pm](https://user-images.githubusercontent.com/454690/34329407-c284c5c2-e8b3-11e7-8c03-d29f5fc98b5c.png)

This opens a dialog. In "Coordinate reference system", select "UTM", then press OK.

![screen shot 2017-12-24 at 2 05 31 pm](https://user-images.githubusercontent.com/454690/34329408-c29c7f28-e8b3-11e7-828f-597d01326a44.png)

All right, now you'll have a blank, georeferenced canvas to work with.

### Import georeferenced path into Open Orienteering Mapper

We're going to use our Runkeeper path as a template to draw paths.

In the "Templates" menu, select "Open template..."

![screen shot 2017-12-24 at 2 03 03 pm](https://user-images.githubusercontent.com/454690/34329405-c2533854-e8b3-11e7-9da2-60743be9492d.png)

Find and open the .gpx file you downloaded from Runkeeper.

It will ask you if you would like to import the template georeferenced or non-georeferenced. You want georeferenced! (That was the whole point.) Click "Georeferenced".

![screen shot 2017-12-24 at 2 03 14 pm](https://user-images.githubusercontent.com/454690/34329409-c2b3dff6-e8b3-11e7-9863-091d53234e79.png)

If nothing shows up on your screen, click "View" and "Show whole map".

![screen shot 2017-12-24 at 2 07 06 pm](https://user-images.githubusercontent.com/454690/34329406-c26db418-e8b3-11e7-9405-bcfc1486c142.png)

This should center your freshly imported template on the screen:

![screen shot 2017-12-24 at 2 20 22 pm](https://user-images.githubusercontent.com/454690/34329452-a002ea18-e8b5-11e7-9e1e-62e45744a3fe.png)

### Tracing trails with Open Orienteering Mapper

I know that in my example pictures, I'm on city streets. But, let's pretend they're trails for the purpose of this exercise.

Using the template, choose a trail symbol and trace the path shown in the template:

![screen shot 2017-12-24 at 2 59 21 pm](https://user-images.githubusercontent.com/454690/34329580-15af8348-e8bb-11e7-90ee-75f1c246ba4e.png)

![screen shot 2017-12-24 at 2 59 12 pm](https://user-images.githubusercontent.com/454690/34329582-15df2530-e8bb-11e7-8235-d6bc76b5927a.png)

Note I walked back and forth on mostly the same path, but the GPS trails are not perfect, overlapping lines. Accuracy is typically within 4.5 meters.

This is very normal for GPS data collection. It's a good idea to collect data a few times so that you can average the GPS trails.

Here is our resulting trail map (after hiding the template)!

![screen shot 2017-12-24 at 2 59 34 pm](https://user-images.githubusercontent.com/454690/34329581-15cb1d4c-e8bb-11e7-9acb-b5544a6db87e.png)

---
Bonus: Check your work by importing an Open Street Map template of the area. [Continue](1.5_Runkeeper_OSM.html) to see the bonus content.
