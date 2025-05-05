# Memory traces

Memory traces is an interactive audio-visual experience that transforms LUKSO blockchain assets into musical sequences and visualizations.

![cables_202555_155555](https://github.com/user-attachments/assets/9db9d650-6fe0-4984-9f33-f4b55433b6aa)

## Overview

Memory traces analyzes Universal Profile assets chronologically to create unique sonic fingerprints of on-chain identity and activity. By retrieving and processing blockchain data, the system generates evolving musical compositions that represent your digital journey on the LUKSO blockchain.

## Features

- **Asset Chronology**: Retrieves Universal Profile assets and orders them based on acquisition time
- **Musical Sonification**: Converts blockchain addresses and transaction data into musical parameters
- **Multi-Voice Synthesis**: Employs a four-voice polyphonic system with customizable waveforms and envelopes
- **Advanced Audio Processing**: Implements stereo ladder filters and spatial audio effects
- **Interactive Visualization**: Synchronizes visual elements with musical sequence playback
- **Drone Generation**: Creates evolving drone sounds to complement the main melodic elements

## Technical Architecture

Memory traces consists of several interconnected components:

1. **Data Acquisition Layer**: Connects to LUKSO RPC endpoints to retrieve Universal Profile data
2. **Processing Layer**: Decodes and chronologically orders asset information
3. **Sonification Layer**: Transforms blockchain data into musical parameters
4. **Synthesis Engine**: Generates audio using the derived musical parameters
5. **Effect Processing**: Enhances the sound with filters, reverb, and spatial positioning
6. **Visualization System**: Creates visual representations synchronized with the audio

## Setup and Usage

- Currently the system relies on a manual input of the LUSKO Universal ID
- During the initialization process, the network calls are being made to aquire all the relevant information
- Due to the regulations of web audio a user interaction is required at the end of the initalization, after which the process starts
- NOTE: at a later point the project will be converted to a Mini app that functions within the LUKSO Universal Profile page

### Prerequisites

- A LUKSO Universal Profile address
- Access to a LUKSO RPC endpoint

### Browser Compatibility
Memory traces relies heavily on the Web Audio API for audio synthesis and processing. Browser support varies:

Chrome/Edge: Best performance and most reliable filter behavior
Firefox: Good overall support but may exhibit differences in filter resonance
Safari: Some features like audio worklets may behave differently
Mobile Browsers: Limited support; performance may vary significantly

For optimal experience, we recommend using the latest version of Chrome or Edge on desktop.

### Installation

1. Clone this repository
2. Install a local NPM server
3. Connect to a LUKSO RPC endpoint
4. Enter your Universal Profile address
5. Generate and play your unique memory traces

## How It Works

Memory traces leverages the ERC725Y data structure to access LSP5ReceivedAssets from Universal Profiles. Assets are retrieved in chronological order using Transfer events from the blockchain, then processed through a parameter mapping system that converts addresses into musical values.

The core of the sonification process involves:

1. Extracting meaningful patterns from asset addresses
2. Mapping these patterns to musical parameters (pitch, duration, timbre)
3. Generating audio using a multi-voice synthesis engine
4. Processing the audio through effects to create spatial depth
5. Visualizing the sequence for an integrated experience

## Development

This project is built on advanced Web Audio API techniques and blockchain interaction methods. Key components include:

- Custom implementation of ERC725.js functions for asset retrieval
- Web Audio oscillators, filters, and effect processors
- Binary search algorithms for efficient asset discovery
- Advanced parameter mapping for musical coherence

## License

CC BY-NC-SA 4.0

## Credits

Created by Jan Ove Hennig as part of the "Abstracted Patterns" program initiated by Refraction DAO / LUKSO

## Acknowledgments

- LUKSO for the Universal Profile standard
- Cables.gl for the development framework
- Web Audio API for audio synthesis capabilities
