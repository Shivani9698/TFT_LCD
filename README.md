# Colorful Text Animation on TFT Display using Arduino

This Arduino sketch creates a colorful text animation on a TFT (Thin-Film Transistor) display. The code generates random colors and displays "INTELITEK", "WELCOME TO", "EDU SOLUTION", and "PVT. LMT.!" in a loop, changing the font color every 200 milliseconds.

## Requirements

- Arduino board (e.g., Arduino Uno)
- TFT display with compatible driver (e.g., ILI9341)
- Appropriate connections between the Arduino and the TFT display

## Libraries Required

- TFT library (typically used for displays with ILI9341 or similar controllers)
- SPI library (usually bundled with the Arduino IDE)

## Setup and Installation

1. Connect the TFT display to your Arduino board using the following pin configuration:
   - CS (Chip Select): Connect to pin 10
   - DC (Data/Command): Connect to pin 9
   - RST (Reset): Connect to pin 8
   - Other necessary connections for power and backlight (refer to your specific TFT display documentation)

2. Make sure the required libraries are installed in your Arduino IDE:
   - TFT library
   - SPI library

3. Upload the provided sketch to your Arduino board using the Arduino IDE.

## How the Code Works

1. The code initializes the TFT library and sets the background color to black.

2. A random color (RGB) is generated for the font using `random()` function.

3. The text "INTELITEK", "WELCOME TO", "EDU SOLUTION", and "PVT. LMT.!" are displayed on the TFT screen with the generated random font color. The text is positioned in the middle of the screen.

4. The code then waits for 200 milliseconds before changing to the next random font color, creating a colorful text animation effect.

5. The loop continues indefinitely, generating random font colors and displaying the text in a loop.

## Important Notes

- The TFT library used in this code may require modification if your TFT display uses a different controller or pin configuration.
- The code assumes that the TFT display supports the `setTextSize()` and `text()` functions. Some TFT libraries might have different function names for text rendering.

## License

This code is provided under the MIT License. See the LICENSE file for more information.

## Author

Created by Shivani Raj. Contact: rajshivani.jh@gmail.com.
