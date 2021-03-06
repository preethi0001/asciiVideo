# asciiVideo
A quick and easy open source python code to convert a video into a work of asciiVideo.

Example gif

![Alt Text](https://media.giphy.com/media/3nl12QTwHM8gXMiyDg/giphy.gif)

Full render of single frame.

![ascii art](https://github.com/mazy1998/asciiVideo/blob/master/fullrender.png?raw=true) 

This is the equivalent of turning a picture into ascii art as but with video. I would like to thank [Christian Diener](https://gist.github.com/cdiener) for his ascii art algorithm  [asciinator](https://gist.github.com/cdiener/10491632) which was the pillar of this project. For new comers [ASCII](https://en.wikipedia.org/wiki/ASCII) is an abbreviation for *American Standard Code for Information Interchange*, which includes all the character the Americans deemed [necessary](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/ASCII-infobox.svg/2880px-ASCII-infobox.svg.png) for a PC when developing computers. 

# How to use asciiVideo.py

1. First run the asciiVideo.py file in the same directory of a video you wish to convert
2. Then create an object with the asciiArt initializer.
	1. ```cat = asciiArt("videoofcat.mp4") ```
3. This will then display a picture of the video frame and its ascii conterpart.
4. From here you can change the gamma of the asciiVideo for more or less details.
	1. ```cat.setGamma(1)``` to add more dark details.
	2. ```cat.setGamma(1.5)``` to get rid of dark details like shadows.
	3. ![gamma comparison](https://github.com/mazy1998/asciiVideo/blob/master/gammacomparison.jpg?raw=true)
5. You can also change the rotation of the video using.
	1. ```cat.setRotation(angle)```
	2. ```cat.setRotation(180)``` can be used on upside down videos
6. When you're happy with your gamma and rotation you can render.
	1. ```cat.render("<outputfile>")```
	2. For example ```cat.render("asciiCatVideo")```
7. If you are satisfied with your video it is wise to close the object.
	1. ```cat.close()```
	2. This gets rid of all unecessary memory used to make the video
8. Finally you can share the video with friends and loved ones.

# How the code works
Terminology | definition 
------------ | -------------
Video Frame | A single instances of video in the form of a picture
Ascii Text | A *video frames* ascii art text in the form of a string
Ascii Frame| An *ascii text* converterd into a picture
Ascii Video | All *ascii frames* compiled into a video

![Flow chart](https://github.com/mazy1998/asciiVideo/blob/master/flowchart.png?raw=true)





