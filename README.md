pjm-moogerfooger - Max for Live device wrappers for Moogerfooger plugins
--------------------------------------------------------------------------------

This is a Max for Live Audio Effect device. It is a wrapper over the [Moog
Moogerfooger plugins], which you must already have installed on your box.

The "skins" for the devices were created by screenshotting the devices on
my computer, and then placing them in the patcher window.  

Each device has a small "up arrow" control near the top left, that can
be used to open the actual plugin to interact with it.

No idea how to get existing factory presets available in the Live device;
you can list them, but not set them.  To use a preset, open the actual
plugin (see above), select the preset, and the Live device's settings
will change to that, so you can create a Live preset for those.

[Moog Moogerfooger plugins]: https://www.moogmusic.com/products/moogerfooger-effects-plug-ins


usage
================================================================================

Copy the `*.amxd` files to your computer, and add to Ableton Live.

details
================================================================================

pjm-MF-101S Filter
--------------------------------------------------------------------------------

![pjm-MF-101S Ableton device](./images/pjm-MF-101S.png)

The auto-mapped parameters for the devices are set up as the following banks
(each row is a bank):

| control 1   | control 2     | control 3    | control 4   | control 5     | control 6   | control 7     | control 8  |   
|-------------|---------------|--------------|-------------|---------------|-------------|---------------|-------------
| env         | follow        | mix          |             | drive         | output      | cutoff        | res        |
| slope       | link          | type         | resp        |               |             |               |            |

The parameter names, with associated Moog name and VST parameter number.

| param  | pjm name | Moog name |
| ------ | -------- | --------- |
|    5   | env      | Envelope Amount |
|    6   | follow   | Envelope Follow Rate |
|    7   | mix      | Envelope Mix |
|    2   | drive    | Drive |
|    3   | output   | Output |
|    8   | cutoff   | Filter Cutoff |
|    9   | slope    | Filter 2-Pole / 4-Pole Switch |
|   10   | res      | Filter Resonance |
|    4   | link     | Link |
|   11   | type     | Envelope Mono / Stereo |
|   12   | resp     | Response Exponential / Smooth |



changelog
================================================================================

version 2022.11.30

- initial version