# timecode

#### OVERVIEW ####
Calculating SMPTE timecode and convert to frame number.

* Version 1.0.0
* 2015.11.3

#### USAGE ####

$1 --> mode(add, sub, convert)  
$2 --> fps  
$3 --> timecode, frame number  
$4 --> timecode, frame number  

###### SAMPLE
timecode -a 30 00:00:30:00 00:00:10:00 --> 00:00:40:00  
timecode -a 30 900 00:00:10:00         --> 00:00:40:00  
timecode -a 30 00:00:30:00 300         --> 00:00:40:00  
timecode -s 30 00:00:30:00 00:00:10:00 --> 00:00:20:00  
timecode -s 30 900 00:00:10:00         --> 00:00:20:00  
timecode -s 30 00:00:30:00 300         --> 00:00:20:00  
timecode -f 30 00:00:10:00             --> 300  
timecode -t 30 300                     --> 00:00:10:00  

###### SUPPORTED FRAME RATE

* 24fps(24)
* 25fps(25)
* 30fps/DF(29)
* 30fps(30)
* 60fps/DF(59)
* 60fps(60)

#### CHANGE LOG ####

* The first release version.
