Created by Marat Bakirov 2013-2021
Discussion
https://forum.ableton.com/viewtopic.php?f=1&t=197828

Releases:

Ableton 11:
https://github.com/maratbakirov/AbletonLive11_MIDIRemoteScripts/releases


Ableton 10:
https://github.com/maratbakirov/AbletonLive10_MIDIRemoteScripts/releases

Ableton 9:
https://github.com/maratbakirov/AbletonLive9_RemoteScripts/releases
Novation_Impulse2_9_1.zip is for older versions 
Novation_Impulse2.zip
is for newer versions


Features

Mixer  button 9 = OverDub
Shift + Mixer  button 9  = Automation record on/off

Shift + Rec  = Metronome on/off
Shift + Play = Undo
Shift + Stop = Stop all clips
Shift + Ffwd/Back  - next/previous device ?? to investigate if it works still

Shift + Loop now enters "alternative assignments" mode.
Differences:
  is that mixer buttons are permanently armed (like the shift is pressed)
  if you press Shift and arm the track, it will NOT me selected automatically

It is very good for perfomance when you need to quickly switch instruments and only have one left hand or right hand available as the other is ready to play

Shift + Clip buttons are now clip stop



Known issues that cannot be fixed
1) After moving track with Shift+Track buttons are not returned to inital condition.
    Also happens sometimes in other cases (like bank switching with Shift).
   Workaround - press and release Shit again.
  update : seems to work fine with Nocation Firmware 695 and higher
2) Pressin shift + (mutes/solos) flip button leds to unpredictable results.
   Workaround - do not do that, if you have done that, just press and release shift.

The reason for these problems is that when you use shift+track or shift+bank, the message "shift off" is not sent.
This is out of the scope of what I can do. The bug report is sent to Novation.

Known issues and todo:
FIXED: 1) impulse does not disconnect properly and does  not send disconnection message.
FIXED  1.5) refactor shift - move it to main class.
FIXED: 2)when track goes down, the bank is not changed.
3) on initialize mute/solo buttons do not light
  workaround - press shift button.
FIXED: 4) when arming a single track make the track selected


Future things to implement.

DONE 1) mixer9 - overdub
DONE 3) Shift + Stop - stop all clips.


FIXED:4) Shift+Mixer9 - Automation record on/off
4.5) Shift + Rec = metronome
5) Shift + Loop switch session/arrangement (as loop is the button that also changes in this case)
   replanned as shift+loop now behave totally differently
FIXED: 6) Shift + play Undo (as play is like backspace but turned opposite)

DONE: another parallel feature - Shift + drum pad in clip mode - stop the selected clip.

think of re-mapping drum pads for another notes.

7) display messages, when
   metronome on/off
   undo
   switch session/arrangement
   overdub
   automation arm

2) Shift + Mixer 9 - automation arm (seems to be rather hard - not sure there is API for that)




# Original
original repo could not be forked as it contained one invalid file 
https://github.com/gluon/AbletonLive11_MIDIRemoteScripts/tree/main/MPK261
*pysudo_dis_failed

this file made it not possible to clone the repo on windows 

# Original readme at 
# https://github.com/gluon/AbletonLive11_MIDIRemoteScripts

# Ableton Live 11 (beta) MIDI Remote Scripts 

Unofficial repository for Ableton Live 11 MIDI Remote Scripts Python Sources decompiled by Julien Bayle

You can find more informations on this page :
https://structure-void.com/ableton-live-midi-remote-scripts/

You can read the PythonLiveAPI extracted documentation :
https://structure-void.com/PythonLiveAPI_documentation/Live11.0.xml

## UPDATED on 4th December 2020

===> **NO support given, ONLY source files !**

===> **Don't contact Ableton for support about this repository**

Please enjoy.

