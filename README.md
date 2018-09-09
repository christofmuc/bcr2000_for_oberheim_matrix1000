
This is a Behringer BCR2000 template for the Oberheim Matrix 1000 synthesizer I made, because the ones I found in the Internet were not really 
sophisticated and most importantly wouldn't deal with negative numbers correctly.

The SYX file contains two presets, ready to be sent to your BCR 2000 via any Sysex capable MIDI tool (e.g. MIDI-OX). 

**WARNING**: As provided, the SYX file will store two presets at preset positions 31 and 32 in your BCR2000, so make sure before you send it
that there is nothing in these two presets you cannot bring back if you need it.

The BCL file located above contains the cleartext instructions in BCL format (an enormous thanks to Mark van den Berg for providing the excellent document 
on the B-Control MIDI Implementation, which can be found at https://mountainutilities.eu/). 

The BCL can be modified by you if you like, for example to change the $store instructions to use different preset slots, 
and then must be converted to SYX format e.g. with the extremely helpful BC-convert tool from https://www.sequencer.de/synth/index.php/BC-Convert.

Detailed information on the layout implemented can be found in the two PDF documents. I am not yet happy with the layout quality, but this was the best 
I could do quickly.


