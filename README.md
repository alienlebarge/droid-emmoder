# Droid Emmoder

_Emmoder_ (pronounced `\ɑ̃.mɔ.de\`) means _to initiate_, _to set in motion_, _to start_ in Swiss-French patois.

A 4-track drum sequencer with algorithmic pattern generation and CV sequencer for the [Droid Universal CV Processor](https://shop.dermannmitdermaschine.de/pages/droid-universal-cv-processor).

## Features

- **4 drum tracks** (Kick, Snare, HiHat, Clap) with algoquencer
- **16-step pattern programming** with 2 controllers
- **Individual and global mute** system
- **CV sequencer** (motoquencer) with 4 faders
- **Automatic clock detection** (external/internal)
- **Page system** for different control modes

## Hardware Requirements

- 1 Master
- 1 G8 (gate outputs)
- 1 P10 (potentiometers)
- 4 P2B8 (buttons/LEDs)
- 1 M4 (faders)

## Installation

Copy the `droid.ini` file to an SD card and load it into your Droid Master module.

## User Manual

### 1. Basic Setup

**Essential connections:**
- **I1**: External clock (optional - uses internal clock by default)
- **I5**: Global reset (optional)
- **G1.1-G1.4**: Drum outputs (Kick, Snare, HiHat, Clap)
- **O2**: Motoquencer CV output
- **O6**: Motoquencer gate output

### 2. Drum Sequencer (Page 1)

**Activation:**
- Press **B5.7** to select the drum page

**Track selection:**
- **B4.1**: Kick
- **B4.3**: Snare  
- **B4.5**: HiHat
- **B4.7**: Clap

The corresponding LED lights up to indicate the selected track.

**Pattern programming:**
- Use buttons **B2.1-B2.8** and **B3.1-B3.8** to program the 16 steps
- LEDs indicate active steps for the selected track
- Step distribution:
  - B2: steps 1, 2, 5, 6, 9, 10, 13, 14
  - B3: steps 3, 4, 7, 8, 11, 12, 15, 16

**Per-track settings:**
- **Activity** (density): P1.3 (Kick), P1.5 (Snare), P1.7 (HiHat), P1.9 (Clap)
- **Variation** (randomness): P1.4 (Kick), P1.6 (Snare), P1.8 (HiHat), P1.10 (Clap)

**Mute system:**
- **Individual mute**: Select track + press **B4.2**
- **Global mute**: **B4.4** (cuts all tracks instantly)

### 3. CV Sequencer (Page 2)

**Activation:**
- Press **B5.8** to select the CV page

**Step configuration:**
- **P5.1**: Number of active steps (1-8 steps)

**CV programming:**
- Use faders **P5.2-P5.4** on the M4 module to set CV values
- Quantized output on **O2** (0.2V range, 2-semitone quantization)

**Page navigation:**
- **B5.7/B5.8**: Toggle between pattern and parameter pages
- **B5.5/B5.6**: Toggle between CV and gate modes

### 4. Clock Control

**Internal tempo:**
- **P1.1**: Controls internal clock speed
- **L4.6**: LED blinks with the tempo

**External clock:**
- Connect your clock to **I1** (automatic detection)
- System automatically switches to external clock when present
- Clock is redistributed on **O1**

**Reset:**
- **I5**: Global reset (synchronizes all sequencers)
- **O5**: Reset output (for chaining other modules)

### 5. User Interface

**Controller 1 (P10):**
- P1.1: Clock speed
- P1.3/4: Activity/Variation Kick
- P1.5/6: Activity/Variation Snare  
- P1.7/8: Activity/Variation HiHat
- P1.9/10: Activity/Variation Clap

**Controller 4 (P2B8 - Track Selection):**
- B4.1: Kick selection
- B4.2: Mute selected track
- B4.3: Snare selection
- B4.4: Global mute
- B4.5: HiHat selection
- B4.7: Clap selection

**Controller 5 (P2B8 - Navigation):**
- B5.7: Page 1 (Drums)
- B5.8: Page 2 (CV)
- B5.5/5.6: Motoquencer modes

### 6. Usage Tips

**Recommended workflow:**
1. Start on the drum page (B5.7)
2. Select a track (B4.1/3/5/7)
3. Program the pattern with step buttons
4. Adjust activity/variation with corresponding potentiometers
5. Repeat for other tracks
6. Use mute for live variations
7. Switch to CV page (B5.8) to add melodies

**Live performance:**
- Global mute (B4.4) allows instant drops
- Activity/variation controls let you evolve patterns in real-time
- Page system allows quick switching between drums and melodies

## Resources

Find other Droid patches on GitHub by searching for the [droid-eurorack](https://github.com/topics/droid-eurorack) topic.

---

Inspired by [Mathias Kettner](https://dmmdm.de/)'s Droid examples.