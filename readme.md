

[RCPNT-FM_0.1]
=========
Pure Data FM synth with Lemur templates for iPad


Description
----
RCPNT-FM_0.1 is a Frequency Modulation Synthesizer built with Pure Data and featuring:
	
* 1 Carrier
* 3 Modulators
* 3 Modulation index couples
* 6 Drawable Envelopes :
	- Global Amp Envelope [envelope looping on release point]
	- Pitch Modulation,
	- Frequency Modulation Ratios 
	- 3 envelopes for modulation indexes.
	- LFO (Hz/ClockDiv)
	- You can set the LFO rates directly in Hz,
    	  depending on the clock (BPM) ,
     	  or on the note duration (n/dur).
	- You can also bind LFO table reading to the Global Envelope LFO.
* 1 ADSR Envelope generator
* 5 selectable basic waveforms and an interface to build them as sine sums.
* A LEMUR Ipad custom INTERFACE with a STEP-SEQUENCER (which you can sync to an EXTERNAL MIDI CLOCK), step-based musical MODE selection, and DRAWABLE ENVELOPES with breakpoint functions. You can play the synth without looking at your laptop screen.


Feel free to play,share and edit!

___________


Package Content:
---------------


* RCPNT-FM-0.1.pd - Frequency Modulation Synthesis Unit
* help-control.pd - help for controllable parameters
* midisbrani - map your midi CCs and send values to your <receive> objects 
* oscsbrani - map your OSC parameters and send values to your <receive> objects
* RCPNTlemur-intclock - "RCPNT-FM" Lemur template with internal clock (still buggy)
* RCPNTlemur-extclock - "RCPNT-FM" Lemur template with external clock sync
___________


Plug and Play:
----
You can play with the custom Lemur template, with any Midi keyboard/device, or arpeggiator. Just plug your device in, open the patch and enjoy. Use IAC drivers to send midi datas from other softwares/DAWs.

Info: 
----

- Check help-control.pd to know more about parameters.
- The UDP port is 8006


Known Problems and limitations: 
----
- Global Envelope Sustain/Loop Precision	
- Lemur Step Sequencer (internal-clock precision)
- LFOs rate ranges not working (on iPad)
- Editing wavetables content while reading with tabosc~ creates audio drop-outs and clicks
- Global Envelope LFO works only in looped parts of the envelope
___________

Future Improvements:
--------

- Presets!
- Lists of Harmonic and Inharmonic c/m Ratios
- Global Envelope Optimization
- Wavetable-morphing(Main Oscillator)
- Solution for sinesum clicks problem
- Filters
- Reverb
- Pitchbend range
- Better ADSR, this one's a bit (Pd interface only)
- Better Lemur Step Sequencer	
- Arpeggiator
- Physics on sliders and bouncing breakpoints for dynamic table editing
- Add editable control ranges (for duration, ratio, index)
- Better midi Clock sync

Credits:
----

- All the pure data hurleur community! Thanks!
- Miller Puckette
- John M. Chowning [The Synthesis of Complex Audio Spectra by Means of Frequency Modulation] 
- Bouncing Multislider taken from the Lemur demo project <IPad-StudioCombo>
- Wave Builder (sines sum) based on PDDP Tutorials
- Control Rate Phasor based on Jamie Bullock's one (lists.puredata)  
- everyone @ Recipient Collective

Links:
----
- http://puredata.hurleur.com/
- http://lists.puredata.info
- http://recipient.cc

----

alessandro@recipient.cc
Recipient Collective 2014
http://recipient.cc


