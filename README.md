# Memory Traces

Memory Traces is an interactive audio-visual experience that transforms LUKSO blockchain assets into musical sequences and visualizations.

![cables_202555_155555](https://github.com/user-attachments/assets/ebb491c4-0f53-46e6-ae80-1bc862a749eb)

## Overview

"Memory Traces" analyzes Universal Profile assets chronologically to create unique sonic fingerprints of on-chain identity and activity. By retrieving and processing blockchain data, the system generates evolving musical compositions that represent your digital journey on the LUKSO blockchain.

## Features

- **Asset Chronology**: Retrieves Universal Profile assets and orders them based on acquisition time
- **Musical Sonification**: Converts blockchain addresses and transaction data into musical parameters
- **Multi-Voice Synthesis**: Employs a four-voice polyphonic system with customizable waveforms and envelopes
- **Advanced Audio Processing**: Implements stereo ladder filters and spatial audio effects
- **Interactive Visualization**: Synchronizes visual elements with musical sequence playback
- **Drone Generation**: Creates evolving drone sounds to complement the main melodic elements

## Technical Architecture

Memory Traces consists of several interconnected components:

1. **Data Acquisition Layer**: Connects to LUKSO RPC endpoints to retrieve Universal Profile data
2. **Processing Layer**: Decodes and chronologically orders asset information
3. **Sonification Layer**: Transforms blockchain data into musical parameters
4. **Synthesis Engine**: Generates audio using the derived musical parameters
5. **Effect Processing**: Enhances the sound with filters, reverb, and spatial positioning
6. **Visualization System**: Creates visual representations synchronized with the audio

## Setup and Usage

### Prerequisites

- A LUKSO Universal Profile address
- Access to a LUKSO RPC endpoint
- Node.js (v14.0.0 or higher)
- Modern web browser (Chrome/Edge recommended)

### Installation and Running

1. Clone this repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the Node.js server:
   ```
   npm start
   ```
4. Open your browser and navigate to `http://localhost:3000`
5. Enter your LUKSO Universal Profile ID in the provided input field
6. Wait for initialization (up to 30 seconds) while network calls are made to acquire blockchain data
7. Interact with the interface when prompted to activate Web Audio (browser requirement)
8. Experience your unique memory traces

### Browser Compatibility

Memory Traces relies heavily on the Web Audio API for audio synthesis and processing. Browser support varies:

- **Chrome/Edge**: Best performance and most reliable filter behavior
- **Firefox**: Good overall support but may exhibit differences in filter resonance
- **Safari**: Some features like audio worklets may behave differently
- **Mobile Browsers**: Limited support; performance may vary significantly

For optimal experience, we recommend using the latest version of Chrome or Edge on desktop.

### Future Development

Note: This project will eventually be converted into a Mini app that functions within the LUKSO Universal Profile page, eliminating the need for manual setup.

### Installation

1. Clone this repository
2. Open the project in cables.gl
3. Connect to a LUKSO RPC endpoint
4. Enter your Universal Profile address
5. Generate and play your unique memory traces

## How It Works

Memory Traces leverages the ERC725Y data structure to access LSP5ReceivedAssets from Universal Profiles. Assets are retrieved in chronological order using Transfer events from the blockchain, then processed through a parameter mapping system that converts addresses into musical values.

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

[Include license information here]

## Credits

Created by [Your Name]

## Acknowledgments

- LUKSO for the Universal Profile standard
- The ERC725 Alliance for the ERC725.js library
- Web Audio API for audio synthesis capabilities
