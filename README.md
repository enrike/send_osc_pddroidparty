License GPL

by ixi-audio.net

This is just a PureData patch that explains how to send OSC messages from a android device by using PdDroidParty app. It requieres the PdDroidParty abstractions installed in the PD path and the app in the android device.

The PdDroidParty app and details on how to use it here
http://www.droidparty.net/


send_osc_example: basic example that allows to set a IP and port, connect/disconnects and shows the connection state, then it sends OSC messages from a slider, a bang, a toggle, and a bonk~ object 
/slider avalue
/go 	1
/toggle 1-0

send_snd_analysis: same as before but it sends data from the analysis of the sound in of the phone. It reports on hit detected sending the volume of the hit, and it also reports on the general amplitude of the sound as well as tries to guess the pitch.
/hit avalue
/pitch afreq
/amp avalue