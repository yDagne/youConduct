# youConduct

<img src="http://www.trbimg.com/img-53e3e2cc/turbine/la-ca-0928-salonen-pg" alt="" width="428">

YouConduct is a set of python script that allow you to conduct an orchestra of virtual instruments. YouConduct is based on two libraries: fluidSynth and OpenCV. FluidSynth is a software that synthesizes music from soundfont in real-time. OpenCV is known for powerful real-time graphics processing.

In order to use youConduct, you need to install the following first:
  - fluidSynth 
  - opencv2
  - python binding for opencv

For debian distributions, you can install the above as follows:

    sudo apt-get install libopencv-dev python-opencv fluidsynth
  
fluidSynth.py is python binding for fluidSynth library which will be used by colorSound.py.

# 1. colorSound.py
colorSound lets you conduct virtual orchestra using colors. It processes images captured from a webcamera and tracks three colors (Green, Blue, and Red). When you run the script, it shows video stream captured from your camera. colorSound detects and tracks the three colors. Only one instance of each color with largest size is tracked, and each color plays different instrument. The soundfont that comes with youConduct ('soundFont1.sf2') has three instrument presets. 

  - Green - Yamaha Grand Piano
  - Blue - Violin
  - Red - Ahh Choir
 
 [![Alt text](https://img.youtube.com/vi/zS5q4DHf4qs/0.jpg)](https://www.youtube.com/watch?v=zS5q4DHf4qs)

Just grab anything that has at least one of the three colors and conduct the orchestra as professionals do. The software can play three instruments simultaneously if it sees all the three colors. Colors can detected from your shirt also!.

You can play other/more instruments by modifying the script to use different soundfont file. If you use different soundfont, make sure that you select the appropriate program and bank for each instrument. 
