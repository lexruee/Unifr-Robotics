Robotics Project [AS2013]
=========================
This repo hosts homeworks of the robotics project at the University of Fribourg.

In this project the [Aseba environment](https://aseba.wikidot.com/en:start) is used to gain some experience in robotics.

##Getting started
Clone this repo using the command:
```
git clone https://github.com/lexruee/Robotics-Unifr
```

Change to the directory homeworks/series_1.

Start Aseba Playground and open the file:
``` 
yoyoWiggle.playground
```
Now start the Aseba Studio and open the file:
```
01_unifr_yoyoWiggle.aesl
```

Load each e-puck file and click on execute (except for e-puck 1).
As a last step click the execute button on e-puck 1 view.

Enjoy!


##Notes on installing Aseba on Ubuntu / Linux mint


- See https://aseba.wikidot.com/forum/t-683599
- See https://aseba.wikidot.com/de:linuxinstall

##Create a .tgz file

For creating a tgz file use the tar command.

Options:

	- -c create a new archive
	- -f use archive file
	- -z gzip files

Example:

Create archive.tar from files foo and bar:
```
tar -cf archive.tar foo bar
```

Create a .tgz file from files foo and bar:
```
tar -czf arhcive.tgz foo bar
```
Note: The option -f must be last the option!
So tar -cfz ... won't work!
