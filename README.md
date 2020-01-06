
# Behringer BCR2000 for Oberheim Matrix 1000 #

This is a Behringer BCR2000 template for the Oberheim Matrix 1000 synthesizer I made, because the ones I found in the Internet were not really sophisticated and most importantly wouldn't deal with negative numbers correctly.

### What's in it ###

The SYX file contains two presets, ready to be sent to your BCR 2000 via any Sysex capable MIDI tool (e.g. MIDI-OX). 

**WARNING**: As provided, the SYX file will store two presets at preset positions 31 and 32 in your BCR2000, so make sure before you send it
that there is nothing in these two presets you cannot bring back if you need it.

The BCL file located above contains the cleartext instructions in BCL format (an enormous thanks to Mark van den Berg for providing the excellent document on the B-Control MIDI Implementation, which can be found at https://mountainutilities.eu/). 

The BCL can be modified by you if you like, for example to change the $store instructions to use different preset slots, 
and then must be converted to SYX format e.g. with the extremely helpful BC-convert tool from https://www.sequencer.de/synth/index.php/BC-Convert.

### Layout ###

Detailed information on the layout implemented can be found in the two PDF documents. I am not yet happy with the layout quality, but this was the best I could do quickly.

### NRPN Version ###

For the newer firmwares 1.16 and 1.20, you can also give the files a try with the filenames ending on _nrpn_ - these do not use Sysex commands, but normal NRPN commands. These are only understood by the newer firmwares, though.

The only advantages over the version with the Sysex I can see is that NRPNs are bound to a MIDI chanel while Sysex is not, so if you have more than one Matrix1000, you can use the channel to separate the two. On the other hand, NRPNs are understood by many devices, so the chances that you are actually editing something else than the Matrix are higher using the NRPN version.

The NRPN is definitely better when you want to record parameter changes in a DAW.

Note that the NRPN Preset is coded for MIDI channel 1 - in case you want a different channel (very likely), you need to change the `.easypar NRPN 1` into e.g. for channel 9 `.easypar NRPN 9` in the BCL file, use BCConvert to recreate the SYX and send that to the BCR2000.


