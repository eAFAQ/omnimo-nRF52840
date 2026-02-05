# Omnimo nRF52840 Board Variant Definitions for the Adafruit nRF52 Arduino Core

The following instructions explain how to add support for the **Omnimo nRF52840** to the **Adafruit nRF52 Arduino core**. This enables the Omnimo nRF52840 to be selected and programmed directly from the **Arduino IDE**.

## Installation Instructions

To add support for the Omnimo nRF52840 to the Adafruit nRF52 Arduino core, make sure the core is installed first. Then, one existing file must be modified and one new folder must be added:

- Modify the `boards.txt` file

- Copy the folder `variants/omnimo_nrf52840`

## 1. Install the Adafruit nRF52 Arduino Core (If Not Installed)

1. Open the Arduino IDE.

2. Go to File → Preferences.

3. In the Additional Boards Manager URLs field, add the following URL (if it is not already present):  
`https://adafruit.github.io/arduino-board-index/package_adafruit_index.json`

4. Click OK.

5. Go to Tools → Board → Boards Manager.

6. Search for Adafruit nRF52.

7. Install “Adafruit nRF52 Boards”.

## 2. Locate the Adafruit nRF52 Core Installation

If the core was installed using the Arduino Boards Manager, it is typically located in one of the following directories:

- **Windows:**  
`%LOCALAPPDATA%\Arduino15\packages\adafruit\hardware\nrf52\<version>`

- **macOS:**  
`~/Library/Arduino15/packages/adafruit/hardware/nrf52/`

- **Linux:**  
`~/.arduino15/packages/adafruit/hardware/nrf52/`

If the core was installed manually in your Arduino sketchbook, it will be located in:  
`hardware/adafruit/nrf52/`

## 3. Update the boards.txt File

1. Open the `boards.txt` file found in the directory above.

2. Scroll to the end of the file.

3. Copy and paste the contents of `eafaq_boards.txt` and append them to the bottom of `boards.txt`.

## 4. Add the Variant Folder

1. Copy the contents of the provided `variants` folder.

2. Paste them into the`variants` directory of the Adafruit nRF52 core.

No existing files should be overwritten. A new directory named variants/omnimo_nrf52840 should be added.

## Directory Contents

- **eafaq_boards.txt**  
Additional board definitions for Omnimo nRF52840

- **variants/omnimo_nrf52840**  
Board-specific definitions for Omnimo nRF52840
