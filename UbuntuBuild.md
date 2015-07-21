First build HeeksCAD for Ubuntu. ( see http://code.google.com/p/heekscad/wiki/CompilingForUbuntu )

Run RapidSVN ( menu Applications->Programming->RapidSVN ) On the RapidSVN menu, choose Repository->Chekcout In the URL box put: http://heeksart.googlecode.com/svn/trunk/ In the "Destination Directory" box, put: /home/dan/Desktop/HeeksArt ( but replace "dan" with your username ) Click "OK". This should get all the source code files you need.

edit /home/dan/.bashrc  ( you'll have to choose "Show Hidden Files" on the View menu to see it )
add

export HEEKSCADPATH=/home/dan/Desktop/HeeksCAD

as the last line


On the Ubuntu menu, click Applications->Accessories->Terminal. The "Terminal" window appears, with some text like "dan@dan-desktop:~$" in it.

Type: cd Desktop/HeeksArt

( if you've already built HeeksArt, you should type: make clean    now because my makefile does not always know which files are out of date )

Then type: make

Look for errors

You can then run HeeksCAD by typing ../HeeksCAD/HeeksCAD or:
On the Ubuntu menu, go to Places->Desktop Then double click on HeeksCAD folder to open it. You will see HeeksCAD with a blue diamond icon. Double click on the blue diamond icon to run HeeksCAD.

In HeeksCAD, on the menu, do File->Plugins
You will need to add a new plugin.

Name: HeeksArt

Filepath: ( browse for the HeeksArt.so.0.1.0, you have to click "..." to browse )

Then close HeeksCAD and run it again.
( this will have made an entry in the configuration file /home/dan/.HeeksCAD, you will have to "Show Hidden Files" to see it )

You should now have a "Mesh" menu entry