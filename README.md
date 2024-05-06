# Splendid Grand Piano

Public Domain samples by AKAI

This samples set was released as public domain in early 2000 by Akai company.
It's a Steinway samples with 4 velocity layers.
The version we put here is the 256 MB version.
All samples has been properly fixed and converted to flac,
and mapped to SFZ format with ARIA extensions by kinwie.

Audio demo : https://sfzinstruments.github.io/pianos/splendid_grand_piano


## Compatibility Notes

This SFZ Instrument is reconstructed with the heavily use of SFZ specification level 2.0 + ARIA Extensions. With this is mind, this 
instrument will only played properly in Plogue sforzando and similar sfz samplers that used ARIA Engine. Trying to play this 
instrument in other than ARIA-based sfz samplers may cause issues and problems if it doesn't support the opcodes superset 
used in this sfz instrument. If ARIA-based sfz sampler is not your choice, we advised you to choose a sfz sampler that has similar 
level of opcodes support for this instrument can be played and sounded as it should.


## Control Details

- Sus.Pedal : Sustain pedal position (up/down)
- Resonance : String resonance amount
- Release : Release time, up to 2 seconds, initial at 0.7 seconds
- Veltrack : Dynamic range / velocity to volume response


## Improvements and Features

- This piano has the note-selfmasking sfz native feature and polyphony optimized. This means, when playing a lot of notes (e.g. 
repetitive, trills or sustain pedal down), the voices count will be handled effectively and lower, which also means less jumping in 
CPU usage and results in more natural piano sound behavior.

- 5th layer added at lowest velocity using filter cutoff.

- High notes are undampened mode only as suggested by all fellow sfz pianist users.

- String Resonance simulation added and active when the sustain pedal is down/pressed. This feature makes this piano sounds 
fuller, thanks to Peter Eastman. Turn down the "Resonance" control to 0 will also turn off the resonance polyphony usage.


## Usage Tips

- Setting Veltrack value to achieve a pleasant dynamic range that suit you also depend on your playing style and your 
keyboard/MIDI controller touch response. Try increase and decrease this "Veltrack" parameter as you play and feel the suitable 
one for you. To change the default value permanently, find this line in the sfz file : `set_hdcc$VELTRACK=1` and change the 
value to the one that you wanted, range from 0 to 1.

- MIDI CC numbers are assigned at the top of the sfz file with the #define macro. They can be quick and easily changed to your personal 
favor or to match your MIDI controller device setup. After loading the instrument in sforzando, click the "Open In Text Editor" 
blue button at the INFO page, the sfz file will open by your default text editor. You will see a list of parameter's defined 
numbers. Change the number to your preference and then save it (e.g. Ctrl+S in WinOS), the CC numbers are updated to new 
ones. This is a handy feature in sfz and is a bit similar to MIDI Learn function.

- If you are an advanced user and well understand this SFZ format, you can also modify anything in this sfz instrument to your 
personal taste, make new presets and settings that suit to your private need. SFZ is an easy-to-learn format and very editable. 
However, if you use this sfz as your basis to create a new one and want to distribute it, we just ask to explicitly put a note that 
it's derived from this sfz instrument in this github repository.


## Update Log

- May 6, 2024 : Add Half-pedalling by Peter Eastman

- Sep 16, 2020 : Add String Resonance simulation created by Peter Eastman

- Aug 23, 2020 : Cosmetic update

- Aug 14, 2020 : Optimizing polyphony

- Jul 9, 2020 : Increase hold and decay time, suggested by Peter Eastman
