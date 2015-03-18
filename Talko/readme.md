##Arduino based Talkie Eurorack Module 
**Have your modular speak out the CV**  

This arduino based module works thanks to a clever library : Talkie from https://github.com/going-digital/Talkie 


![Early Panel](https://raw.githubusercontent.com/deladriere/euro-modules/master/Talko/Img/panel.jpg)


####Intro 
Realtime lpc synthesis
no sampling 
realiable to produce intelligible voice or ... not : your choice
tempo aware via gate trigger

####Functions
####Bank
For the moment I have added 4 sound banks :
0: digits (from 0 to 9) male voice  
1: digits (from 0 to 9) female voice  
2: Spell the alphabet  
3: nato alphabet  
4: vocabulary  
5: big numbers  
6: voltmeter (reading the CV voltage)  
7: frequencemeter (just saying "Hertz" instead of "Volts")  
8: counter (each gate trigger increments the counter while any cv change resets it)
9: number radio (each gate trigger a 4 number sequence while any cv trigger a new "transmission")
10: time since cv reset  (each gate triggers saying the time in minutes/seconds while any cv change resets the clock to zero)



####CV

CV signal choose the words or phrases to be said

####Gate

Level high start the complete sound in trigger mode. (regardless of it's length)  
If the trigger switch is off, the gate will start the sound and hold it as long as the gate level stays up. Very useful to create crazy rhythms.


####Trigger

Choose between trigger mode or loop mode
In trigger mode the speech has the priority will complete before starting again on a new gate going high signal.  
In loop mode the gate has the piority and the speech can be shopped by a low gate level or can be looped with a high gate level.  

#####Bend

If bend is on, the bend pot ... well, distords the sound.

####Speed

Change the speed of the voice

####Pitch

Change the pitch of the voice

### Progress
October 2014 
- very early prototyping
- breadboard version

January 2015
- first pcb version

### Todo
* publish schematic @done(2014-12-30)
* publish pcb @done(2014-12-30)
* add picture of panel & pcb
* merge library in main code 
* add R/shottky in  with entries for protection @done(2014-11-30)
* add mousers ref to each part (mouser cart : link)
* Add female voice @done(2014-12-30)


more info here : http://elek101.blogspot.be/2014/10/talkie-eurorack-module-part-1-concept.html

http://elek101.blogspot.be/2014/12/talkie-eurorack-module-part-2-schematic.html

####Licence

Jean-Luc Deladrière, Hanabi SPRL 2006-2014.  
Except where otherwise noted, content on this site is licensed under a cc-by-sa 3.0 license.

