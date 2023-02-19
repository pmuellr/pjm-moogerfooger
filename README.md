pjm-moogerfooger - Max for Live device wrappers for Moogerfooger plugins
--------------------------------------------------------------------------------

This is a Max for Live Audio Effect device. It is a wrapper over the [Moog
Moogerfooger plugins], which you must already have installed on your box.

The "skins" for the devices were created by screenshotting the devices on
my computer, and then placing them in the patcher window.  

Each device has a small "up arrow" control near the top left, that can
be used to open the actual plugin to interact with it.

I attempted to deal with presets, but ... it's a mess.  I think what I
finally found was that selecting a preset did not reflect the parameter
changes back to Max, so ... it *would* change the device settings, but
then the device settings no longer matched the view in Live.

[Moog Moogerfooger plugins]: https://www.moogmusic.com/products/moogerfooger-effects-plug-ins


usage
================================================================================

Download the [latest version](https://github.com/pmuellr/pjm-moogerfooger/archive/refs/heads/main.zip).

Extract the contents of the archive, and drag the `*.amxd` files to your 
User Library.  Or whatever it is you do with your `*.amxd` files.

details
================================================================================

pjm-MF-101S Filter
--------------------------------------------------------------------------------

![pjm-MF-101S Ableton device](./images/pjm-MF-101S.png)

The Link Gains, Envelope Type, and Envelope Response controls are the
toggle buttons under the Output knob.

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name | Moog name |
| ------ | -------- | --------- |
|    2   | drive    | Drive |
|    3   | output   | Output Level |
|    4   | link     | Link Gains |
|    5   | env      | Envelope Amount |
|    6   | follow   | Follow Rate |
|    7   | mix      | Mix |
|    8   | cutoff   | Cutoff |
|    9   | slope    | Slope |
|   10   | res      | Resonance |
|   11   | type     | Envelope Type |
|   12   | resp     | Envelope Response |
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| env         | follow        | mix          | slope       | drive         | output      | cutoff        | res        |
| link        | type          | resp         | slope       |               |             |               |            |

--------------------------------------------------------------------------------

pjm-MF-102S Ring Modulator
--------------------------------------------------------------------------------

![pjm-MF-102S Ableton device](./images/pjm-MF-102S.png)

The LFO Sync control is the toggle to the left of the LFO Waveform
button. The Link Gains and LFO Polarity controls are the toggles beneath
the Output knob.  The Carrier Type control is the menu below the LFO
Polarity toggle.

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name | Moog name |
| ------ | -------- | --------- |
|      2 | drive    | Drive |
|      3 | output   | Output Level |
|      4 | link     | Link Gains |
|      5 | lfo      | LFO Amount |
|      6 | waveform | LFO Waveform |
|      7 | rate     | LFO Rate |
|      8 | sync     | LFO Sync |
|      9 | mix      | Mix |
|     10 | range    | Frequency Range |
|     11 | freq     | Frequency |
|     12 | carrier  | Carrier Type |
|     13 | polarity | LFO Polarity |
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| lfo         | waveform      | rate         | drive       | output        | mix         | range         | freq       |

--------------------------------------------------------------------------------

pjm-MF-103S 12-Stage Phaser
--------------------------------------------------------------------------------

![pjm-MF-103S Ableton device](./images/pjm-MF-103S.png)

The LFO Sync control is the toggle to the left of the LFO Range
button. The Link Gains and LFO Type controls are the toggles beneath
the Output knob.  The Output Mode control is the menu below the LFO
Type toggle.

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name | Moog name |
| ------ | -------- | --------- |
|      2 | drive    | Drive |
|      3 | output   | Output Level |
|      4 | link     | Link Gains |
|      5 | lfo      | LFO Amount |
|      6 | range    | LFO Range |
|      7 | rate     | LFO Rate |
|      8 | sync     | LFO Sync |
|      9 | sweep    | Sweep |
|     10 | stages   | Stages |
|     11 | res      | Resonance |
|     12 | mode     | Output Mode |
|     13 | type     | LFO Type |
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| lfo         | range         | rate         | sync        | drive         | output      | sweep         | res        |
| stages      | link          | mode         | type        |               |             |               |            |

--------------------------------------------------------------------------------

pjm-MF-104S Analog Delay
--------------------------------------------------------------------------------

![pjm-MF-104S Ableton device](./images/pjm-MF-104S.png)

The Time Sync control is the toggle to the left of the Delay Range
switch (short/long). The LFO Sync control is the toggle to the right of
the LFO Rate knob. The Link Gains control is the toggle beneath
the Mix knob.

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name      | Moog name |
| ------ | ------------- | --------- |
|      2 | drive         |  Drive              
|      3 | output        |  Output Level                     
|      4 | link          |  Link Gains                   
|      5 | mix           |  Mix            
|      6 | time          |  Time             
|      7 | range         |  Range              
|      8 | feedback      |  Feedback                 
|      9 | delaySync     |  Delay Sync                   
|     10 | lfoWaveform   |  LFO Waveform                     
|     11 | lfoRate       |  LFO Rate                 
|     12 | lfoAmount     |  LFO Amount                   
|     13 | lfoSync       |  LFO Sync                 
|     14 | delayType     |  Delay Type                   
|     15 | tone          |  Tone             
|     16 | timing        |  Timing               
|     17 | lfoPolarity   |  LFO Polarity                     
|     18 | bypassMode    |  Bypass Mode                    
|     19 | feedbackMode  |  Feedback Mode                      
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| time        | feedback      | lfoWaveform  | lfoRate     | lfoAmount     | drive       | output        | mix        |

--------------------------------------------------------------------------------

pjm-MF-105S MuRF (Multiple Resonant Filter Array)
--------------------------------------------------------------------------------

![pjm-MF-105S Ableton device](./images/pjm-MF-105S.png)

The Sync button is the toggle to the left of the Envelope knob.  The
Link Gains control is the toggle to the right of the Output knob. The
three toggles to the right of the Rate knob are Mode, Envelope Peaks,
and Envelope Mode.

Note that the "Pattern Editor" in the "back side" of the plugin is
not controllable via the plugin, so there are no controls for it.

There's something funky going on with the filter sliders.  You can't
drag them.  Only click somewhere on the slider line.  Grumble ...

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name      | Moog name |
| ------ | ------------- | --------- |
|      2 | drive         |  Drive
|      3 | output        |  Output Level
|      4 | link          |  Link Gains
|      5 | mix           |  Mix
|      6 | env           |  Envelope
|      7 | pattern       |  Pattern
|      8 | rate          |  Rate
|      9 | lfo           |  LFO
|     10 | freq          |  Frequency
|     11 | filter1       |  Filter 1
|     12 | filter2       |  Filter 2
|     13 | filter3       |  Filter 3
|     14 | filter4       |  Filter 4
|     15 | filter5       |  Filter 5
|     16 | filter6       |  Filter 6
|     17 | filter7       |  Filter 7
|     18 | filter8       |  Filter 8
|     19 | bpmSync       |  BPM Sync
|     20 | mode          |  Mode
|     21 | envPeaks      |  Envelope Peaks
|     22 | envMode       |  Envelope Mode
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| drive       | mix           | output       | env         | pattern       | rate        | bpmSync       | lfo        |
| filter 1    | filter 2      | filter 3     | filter 4    | filter 5      | filter 6    | filter 7      | filter 8   |


--------------------------------------------------------------------------------

pjm-MF-106S 
--------------------------------------------------------------------------------

There never was a MF-106 device!

--------------------------------------------------------------------------------


pjm-MF-107S Freqbox
--------------------------------------------------------------------------------

![pjm-MF-107S Ableton device](./images/pjm-MF-107S.png)

The Time Sync control is the toggle to the left of the Delay Range
switch (short/long). The Oscillator control is the toggle below that. The 
Envelope Controls control is the toggle below that.

<!--
VST parameter number, parameter names, with associated Moog name:

| param  | pjm name      | Moog name |
| ------ | ------------- | --------- |
|      2 | drive         |  Drive
|      3 | output        |  Output Level
|      4 | link          |  Link Gains
|      5 | freq          |  Frequency
|      6 | sync          |  Sync
|      7 | waveform      |  Waveform
|      8 | env           |  Envelope Amount
|      9 | fm            |  FM Amount
|     10 | mix           |  Mix
|     11 | osc           |  Oscillator
|     12 | envControls   |  Envelope Controls
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| freq        | sync          | waveform     | env         | fm            | mix         | drive         | output     |

--------------------------------------------------------------------------------

pjm-MF-108S ClusterFlux
--------------------------------------------------------------------------------

![pjm-MF-108S Ableton device](./images/pjm-MF-108S.png)

The LFO Sync control is the toggle to the right of
the LFO Rate knob. The Link Gains control is the toggle beneath
the Mix knob.

<!--
VST parameter number, parameter names, with associated Moog name:

| param | pjm name     | Moog name |
| ------| ------------ | --------- |
|     2 | drive        | Drive        |
|     3 | output       | Output       |
|     4 | link         | Link Gains   |
|     5 | mix          | Mix          |
|     6 | time         | Delay Time   |
|     7 | range        | Range        |
|     8 | feedback     | Feedback     |
|     9 | lfoWaveform  | LFO Waveform |
|    10 | lfoRate      | LFO Rate     |
|    11 | lfoAmount    | LFO Amount   |
|    12 | lfoSync      | LFO Sync     |
|    13 | delayType    | Delay Type   |
|    14 | tone         | Tone         |
|    15 | timing       | Timing       |
|    16 | phase        | Out Of Phase |
|    17 | lfoPolarity  | LFO Polarity |
-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| time        | feedback      | lfoWaveform  | lfoRate     | lfoAmount     | drive       | output        | mix        |

--------------------------------------------------------------------------------

pjm-MF-109S Saturator
--------------------------------------------------------------------------------

![pjm-MF-109S Ableton device](./images/pjm-MF-109S.png)

The Link Gains control is the toggle beneath the Output knob.

<!--
VST parameter number, parameter names, with associated Moog name:

| param | pjm name     | Moog name |
| ------| ------------ | --------- |
|    2  | drive        | Drive                |
|    3  | env          | Envelope Amount      |
|    4  | follow       | Follow Rate          |
|    5  | envSens      | Envelope Sensitivity |
|    6  | output       | Output Level         |
|    7  | link         | Link Gains           |
|    8  | tone         | Tone                 |
|    9  | color        | Color                |
|   10  | noiseEnv     | Noise Env. Amount    |
|   11  | envType      | Envelope Type        |
|   12  | envResponse  | Envelope Response    |
|   13  | noiseFilter  | Noise Filter         |
|   14  | noiseType    | Noise Type           |

-->

Auto-mapped parameters as the following banks:

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| env         | follow        | envSens      | tone        | color         | noiseEnv    | drive         | output     |



changelog
================================================================================

version 2023.02.19

- finished MF-105S, MF-108S, MF-109S woot

version 2023.02.18

- finished MF-104S
- finished MF-107S
- touch ups for MF-102S, MF-103S

version 2023.02.17

- finished MF-103S
- plugin names changed, or `vst~` changed; plugin names updated so they load
- added version labels to the plugins; will I remember to update? :-)

version 2022.12.03

- finished MF-101S and MF-102S

version 2022.11.30

- initial version