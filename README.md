# Droid Emmoder Pro

A powerful performance sequencer for Eurorack built around the [Droid universal CV processor](https://shop.dermannmitdermaschine.de/pages/droid-universal-cv-processor).

_Emmoder_ pronounced `\ɑ̃.mɔ.de\` means _to initiate_, _to set in motion_, _to start_ in Swiss-French patois.

![Droid Emmoder Pro](https://github.com/alienlebarge/droid-emmoder/raw/main/emmoder-pro.jpg)

## Overview

Emmoder Pro is a complete performance sequencer that combines:
- 4 independent drum tracks with algorithmic variations
- 2 melodic sequencers with scale quantization
- Multi-pattern storage system
- Performance controls for live manipulation

## Hardware Requirements

This patch requires the following Droid modules:
- 1 Master
- 1 G8 (for drum triggers)
- 1 P10 (for main controls)
- 4 P2B8 (for step sequencing and track selection)
- 1 M4 (for additional outputs)

## Installation

1. Download the `droid.ini` file
2. Copy it to an SD card
3. Insert the SD card into your Droid Master module
4. Power up your system

## Connections

### Inputs
- **I1**: Clock input
- **I5**: Reset input
- **I2**: CV Input 1 (for future expansion)
- **I6**: CV Input 2 (for future expansion)

### Outputs
- **O1**: Clock output (mirrors input clock or internal clock)
- **O5**: Reset output (mirrors input reset)
- **O2/O6**: Melody 1 (CV/Gate)
- **O3/O7**: Melody 2 (CV/Gate)
- **O4/O8**: Accent (CV/Gate)

### Gate Outputs (G8 module)
- **G1.1**: Kick trigger
- **G1.2**: Snare trigger
- **G1.3**: HiHat trigger
- **G1.4**: Clap trigger

## User Interface

Emmoder Pro is organized into four main pages:

### Page 1: Drums
- Select and program drum patterns
- Control activity and variation for each drum track
- Mute individual tracks

### Page 2: Melody 1
- Program the first melodic sequence
- Control steps, scale, and probability
- Set transposition

### Page 3: Melody 2
- Program the second melodic sequence
- Control steps, scale, and probability
- Set transposition

### Page 4: Performance
- Control swing amount
- Visual feedback for active patterns
- Performance tools

## Controls Guide

### Global Controls
- **P1.1**: Clock Speed (when using internal clock)
- **P1.2**: Fine Tempo adjustment
- **P4.1**: Pattern Select (8 patterns available)
- **B5.1-B5.4**: Page selection buttons
- **B5.7-B5.8**: Quick Pattern A/B selection

### Drum Controls (Page 1)
- **P1.3/P1.4**: Kick activity/variation
- **P1.5/P1.6**: Snare activity/variation
- **P1.7/P1.8**: HiHat activity/variation
- **P1.9/P1.10**: Clap activity/variation
- **B4.1/B4.3/B4.5/B4.7**: Track selection buttons
- **B4.2**: Mute button (works with track selection)
- **B2.x/B3.x**: 16-step sequencer buttons

### Melody Controls (Pages 2 & 3)
- **P5.1**: Number of steps
- **P5.2**: Scale/Quantization selection
- **P5.3**: Probability (randomness)
- **P4.2/P4.3**: Transpose Melody 1/2
- **B5.5/B5.6**: Mode selection (Pitch/Random)

### Performance Controls (Page 4)
- **P5.4**: Swing amount
- **P4.4**: Accent level
- **LED feedback**: Visual indicators for active patterns and gates

## Pattern Programming

### Drum Patterns
1. Select Page 1 (B5.1)
2. Select a drum track (B4.1/B4.3/B4.5/B4.7)
3. Program steps using the 16 buttons (B2.x and B3.x)
4. Adjust activity and variation with the corresponding potentiometers

### Melody Patterns
1. Select Page 2 or 3 (B5.2 or B5.3)
2. Set the number of steps with P5.1
3. Choose a scale with P5.2
4. Adjust probability with P5.3
5. Use the mode buttons (B5.5/B5.6) to switch between pitch and random modes
6. Transpose with P4.2 or P4.3

## Performance Tips

1. **Multiple Patterns**: Store up to 8 different patterns using P4.1
2. **Quick Pattern Switching**: Use B5.7 and B5.8 for instant A/B pattern switching
3. **Muting**: Hold B4.2 while pressing a track selection button to mute/unmute
4. **Swing**: Add groove to your patterns with the swing control (P5.4 on Page 4)
5. **Accent**: The accent system automatically generates accents from drum triggers

## Advanced Features

### Algorithmic Variations
Each drum track has an activity and variation control:
- **Activity**: Controls the density of triggers
- **Variation**: Introduces algorithmic variations to the pattern

### Probability
The melodic sequencers include probability controls that introduce randomness:
- At 0%, the sequence plays exactly as programmed
- At 100%, notes have a 50% chance of triggering

### Swing
Add human feel to your sequences with the swing control:
- At 0%, timing is perfectly even
- Higher values push every second step later in time

## Credits

Emmoder Pro was created by alienlebarge (https://alienlebarge.ch)
Parts of the code are inspired by [Mathias Kettner](https://dmmdm.de/) Droid examples.

## Find Other Droid Patches

Find more Droid patches by searching for repositories with the [droid-eurorack](https://github.com/topics/droid-eurorack) topic on GitHub.
