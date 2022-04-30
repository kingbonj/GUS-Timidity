# GUS-Timidity
Gravis Ultrasound Soundfont and Configuration Files for Timidity and/or VLC

## Files
- **timidity.cfg**
- **eawpats.cfg**

## Prerequisites

- _eawpats.sf2_<br/>Available from: https://midis.fandom.com/wiki/Eawpats.sf2_(Gravis_Ultrasound)<br/>
- Timidity++ <br/>`sudo apt install timidity`
- VLC Media Player

## Timidity++ GUS Soundfont 
- Copy _timidity.cfg_ and _eawpats.cfg_ to `/etc/timidity/`
- Copy _eawpats.sf2_ to `/usr/share/sounds/sf2/`
- Open your MIDI file with `timidity /your_dir/*.mid`

## VLC GUS Soundfont
- Install the fluidsynth plugin:<br/>`sudo apt install vlc-plugin-fluidsynth`
- Copy eawpats.sf2 to `/usr/share/sounds/sf2`
- Open VLC's preferences. 
- Select 'All' to see all preferences. 
- Navigate to Input/Codecs > Audio codecs > FluidSynth 
- Browse for and select the eawpats.sf2 file
- Open your MIDI file with `vlc /your_dir/*.mid`

## Additional Soundfonts
- Install some sound fonts to `/usr/share/sounds/sf2` using apt: <br/>`sudo apt install fluid-soundfont-gs fluid-soundfont-gm` 
