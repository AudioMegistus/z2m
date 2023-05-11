z2m (Zoom G3 to midi foot controller)


------------------------------------------------
Click the green code button (top-right) and choose "download zip". Run z2m.exe in z2m folder.
[if you are on Mac or Linux, you should be able to run z2m-master/source/z2m.py if you have python installed.]

This repo is a fork of: https://github.com/carling65/z2m
you will find original instructions there.
------------------------------------------------
<h3><b>My own experience with this script (tested in Win 10/11 only) is a little different to what is described in the original repo:</b></h3>
------------------------------------------------

Basically, just run z2m.exe and you can then select "Zoom G series" as your MIDI input and you should see sysex coming in.
For some reason (I don't know Python well enough to say why), the script does not send Control Change to LoopMIDI Port, but you can script your own translations with Bome MIDI pro or in python, etc.
 
 - YOU DO NOT NEED TO SET ALL EFFECTS TO T.SCREAM
 - YOU DO NOT NEED TO HAVE ALL FOOTSWITCHES OFF

(with appropriate translation)
- You can assign all three knobs on all 6 effects to different Control Change numbers
- Depending on which effect you have selected, the extra knob assignments on page 2 and page 3 of each effect also send individual messages, so you can have up to 9 assigned knobs per effect.

  HOWEVER...

There seem to be two major limitations:
1. the expression pedal (if you have a G3X) does not send any MIDI info at all.
2. the "on" messages for the footswitches are different depending on what order they are pressed. This means that it is more-or-less impossible to assign a consistent Control Change number to the footswtiches.

TODO:
I am planning an Arduino-based hack of my G3X to bring the footswtiches and expression pedal into play.
