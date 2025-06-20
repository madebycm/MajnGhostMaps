# MajnGhostMaps

Ableton Live control surface script for MIDI controllers

## Overview

MajnGhostMaps provides seamless integration between any MIDI controller and Ableton Live, enabling direct control of device parameters through MIDI CC messages.

## Features

- **Device Control**: First 6 knobs mapped to control selected device parameters
  - CC23: Device Parameter 1
  - CC24: Device Parameter 2
  - CC25: Device Parameter 3
  - CC26: Device Parameter 4
  - CC27: Device Parameter 5
  - CC28: Device Parameter 6

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
- `Encoder1-6`: CC numbers for device control (default: 23-28)

## Default CC Mappings

- **CC23-28**: Device parameters 1-6
- **CC1-9**: Track volume faders 1-9

## Usage

Once configured, your MIDI controller will automatically control parameters of any selected device in Ableton Live, similar to how Push controllers work.

## Author

@author madebycm (2025)