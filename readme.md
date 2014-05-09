

[RCPNT-FM_0.1]
=========
Pure Data FM synth with Lemur templates for iPad


Description
----
RCPNT-FM_0.1 is a Frequency Modulation Synthesizer built with Pure Data and featuring:
	
* 1 Carrier
* 3 Modulators
* 3 Modulation indexes couples
* 6 Drawable Envelopes :
	- 1 Global Amp Envelope [envelope looping on release point]
	- 1 for Pitch Modulation,
	- 1 for Frequency Modulation Ratios,
	- 3 for modulation indexes.
	- LFO
	- You can set the LFOs rates directly in Hz
    - dependent on the clock (BPM) 
    - or on the note duration (n/dur).
	- You can also tie LFO tables reading to Global Envelope one.
* 1 ADSR Envelope generator
* 5 selectable basic waveforms and an interface to build them as sine sums.
* A LEMUR Ipad custom INTERFACE with a STEP-SEQUENCER (you can sync to an EXTERNAL MIDI CLOCK), step-based musical MODES selection, and DRAWABLE ENVELOPES with breakpoint functions. You can play the synth without looking at your laptop screen.


Feel free to play,share,edit!

___________

Frequency Modulation Algorithm :
----

Based on John Chowning's old but fundamental paper "The Synthesis of Complex Audio Spectra by Means of Frequency Modulation"



Plug and Play:
----
You can play with the custom Lemur template, with any Midi keyboard/device, or arpeggiator. Just plug your device in, open the patch and enjoy. Use IAC drivers to send midi datas from other softwares/DAWs.

Info: 
----

- Check help-control.pd to know more about parameters.
- Port for OSC stream is 8006


Package Content:
---------------


* RCPNT-FM-0.1.pd - Frequency Modulation Synthesis Unit
* help-control.pd - help for controllable parameters
* midisbrani - map your midi CCs and send values to your <receive> objects 
* oscsbrani - map your OSC parameters and send values to your <receive> objects
* RCPNTlemur-intclock - "RCPNT-FM" Lemur template with internal clock (still buggy)
* RCPNTlemur-extclock - "RCPNT-FM" Lemur template with external clock sync
___________

Known Problems and limitations: 
----
- Global Envelope Sustain/Loop Precision	
- Lemur Step Sequencer (internal-clock precision)
- LFOs rate ranges change still not working
- Editing wavetables content while reading with tabosc~ creates audio drop-outs and clicks
- Global Envelope LFO works only in looped parts of the envelope
___________

Future Improvements:
--------

- Presets!
- Lists of Harmonic and Inharmonic c/m Ratios
- Global Envelope Optimization
- Wavetable-morphing(Main Oscillator)
- Solve sinesum clicks problem
- Filters
- Reverb
- Pitchbend range
- Better ADSR, this one's a bit (Pd interface only)
- Better Lemur Step Sequencer	
- Arpeggiator
- Physics on sliders and bouncing breakpoints for dynamic tables editing
- Add editable control ranges (for duration, ratios, indexes)
- Better midi Clock sync

Credits:
----

- All the pure data hurleur community! Thanks!
- Miller Puckette
- John M. Chowning [The Synthesis of Complex Audio Spectra by Means of Frequency Modulation] 
- Bouncing Multislider taken from Lemur demo project <IPad-StudioCombo>
- Waves Builder (sines sum) based on PDDP Tutorials
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


