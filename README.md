# IA-Interim-Report
Arpeggiator codes for the Interim Report.

This repository contains two arpeggiator scripts:

1.  The live arpeggiator script is designed to work with live input from a MIDI device.
    It interacts with new MIDI data inputs with priority given to new inputs. This means
    that any new input to the device, be it Note ON or Note OFF, overrides and restarts the
    current sequence.
    
2.  The data arpeggiator script is designed to work with data fed to it as a function. 
    It arpeggiates all of the notes fed to it in a string.
    
    
Both arpeggiators have tempo, beat sub-divisions and note shape as inputs. These are standard sequencer controls.

In both cases the file beginning with "state_of_the_arp..." is the main file.
The markov chain file will produce chord change sequences and send them to the audio output of the device when run. 
