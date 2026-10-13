# EyeMelody

**Look at a color, play a note.** A head-mounted eye-tracking instrument for people who cannot use their hands or their voice.

🏆 **QNX Challenge winner, Hack the North**

▶️ **[Watch the demo video](https://youtu.be/8T5pSdE79tU)**

<!-- TODO: add a photo or GIF of the headset in use, e.g. docs/demo.gif, then uncomment: -->
<!-- ![EyeMelody in use](docs/demo.gif) -->

## What it does

The headset has two cameras: one watches your eye, the other watches the table in front of you. Colored objects are placed on the table. **Looking at an object plays a note**, and that is the whole interface.

- **5 supported colors**, enough for most modern pop songs.
- A note fires when you look at an object. Look away and back to play the same note again.
- The table is the layout of the instrument. Arrange the objects however you want, and help someone compose in physical space.
- Configuration, song creation and tempo also happen through gaze, using a blink menu with three options per menu.

Latency from gaze to note is about **100–200 ms**.

### Hardware

- Raspberry Pi 5 running QNX 8.0, worn on the body
- Two Camera Module 3 cameras on the headset (one on the eye, one facing forward), captured through the QNX sensor framework (`libcamapi`)
- Direct Ethernet connection
- Audio plays on a phone or laptop, because the Raspberry Pi 5 has no audio jack

