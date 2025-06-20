# MajnGhostMaps

Ableton Live control surface script for MIDI controllers

## Overview

MajnGhostMaps provides seamless integration between any MIDI controller and Ableton Live, enabling direct control of device parameters through MIDI CC messages.

## Features

- **Device Control**: Split mapping to avoid overriding common device parameters
  - Parameters 1-3: Controlled by CC105-107 (first 3 macros)
  - Parameter 4: Intentionally skipped with dummy CC127
  - Parameters 5-7: Controlled by CC102-104 (macros 5-7)
  
This split configuration prevents accidentally overriding the first parameters on devices when switching between them, while still providing control over 6 key parameters.

## Installation

1. Copy the `MajnGhostMaps` folder to your Ableton Live User Remote Scripts directory:
   - **macOS**: `~/Library/Preferences/Ableton/Live x.x.x/User Remote Scripts/`
   - **Windows**: `C:\Users\[Username]\AppData\Roaming\Ableton\Live x.x.x\Preferences\User Remote Scripts\`

2. Restart Ableton Live

3. Go to Preferences → Link/Tempo/MIDI
   - Select "MajnGhostMaps" from the Control Surface dropdown
   - Set Input/Output to your MIDI controller ports

## Configuration

The script uses MIDI channel 1 by default. To modify the configuration, edit `UserConfiguration.txt`:

- `GlobalChannel`: MIDI channel (0-15, default: 0 = channel 1)
- `Encoder1-6`: CC numbers for device control (default: 102-107)

## Default CC Mappings

- **CC105-107**: Device parameters 1-3
- **CC127**: Dummy mapping for parameter 4 (prevents accidental override)
- **CC102-104**: Device parameters 5-7
- **CC1-9**: Track volume faders 1-9

## Usage

Once configured, your MIDI controller will automatically control parameters of any selected device in Ableton Live, similar to how Push controllers work.

## Author

@author madebycm (2025)