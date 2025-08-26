# MVMP Voice Authentication

This project implements **voice-based authentication** using an **Edge Impulse model** deployed on the **Arduino Nano 33 BLE Sense**.  
It captures audio through the built-in microphone, processes it with the Edge Impulse SDK, and performs real-time classification for authentication.

## Project Structure
MVMP-Voice-Authentication/
├── arduino-code/
│ ├── src/ # Source files from Edge Impulse export
│ ├── edge-impulse-sdk/ # Edge Impulse SDK
│ ├── libraries/ # Arduino libraries
│ ├── nano_ble33_sense_microphone/ # Microphone driver code
│ ├── MVMP_main.ino # Main program (renamed from Edge Impulse export)
│ └── edge_spotting.ino # Additional Arduino sketch
├── documentation/ # Notes, design docs
├── results/ # Training/testing results
├── hardware-setup/ # Photos and diagrams of setup
└── README.md # Project description

##  Setup Instructions

### 1. Hardware Required
- Arduino Nano 33 BLE Sense  
- USB Cable  
- Computer with Arduino IDE installed  

### 2. Software Required
- [Arduino IDE](https://www.arduino.cc/en/software)  
- Edge Impulse exported Arduino library (already included in `src/` and `edge-impulse-sdk/`)  

### 3. Install Arduino Libraries
Make sure the following libraries are installed via **Arduino Library Manager**:
- Arduino_LSM9DS1  
- ArduinoBLE  
- EloquentTinyML  
- Any dependencies included in the `libraries/` folder  

### 4. Running the Project
1. Open Arduino IDE.  
2. Open `arduino-code/MVMP_main.ino`.  
3. Select **Board** → `Arduino Nano 33 BLE Sense`.  
4. Select the correct **Port** under Tools.  
5. Click **Verify** to compile the code.  
6. Click **Upload** to flash it to the board.  
7. Open the **Serial Monitor** at `115200 baud`.  
8. Speak into the Nano’s microphone — results of authentication will be displayed.

##  Results
Add your training/testing accuracy results here once you complete experiments.

##  Hardware Setup
Add photos/diagrams of your Nano 33 BLE Sense connected for testing.

##  Acknowledgements
- [Edge Impulse](https://edgeimpulse.com/) for model training and Arduino export.  
- Arduino community for open-source libraries.  
