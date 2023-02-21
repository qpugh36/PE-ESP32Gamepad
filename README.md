# PE-ESP32Gamepad
This code sets up an ESP32-based gamepad that includes buttons, thumbsticks, and LEDs. The LEDs are controlled using the FastLED library, and the buttons and thumbsticks are read using the Arduino digital and analog input pins.

The program starts by initializing the buttons and thumbsticks as inputs and the LEDs using the FastLED library. The Bluetooth server is also started using the BLEDevice and BLEServer libraries.

The loop function then reads the state of the buttons and thumbsticks and applies a dead zone to the thumbsticks to ensure that small movements are not registered. The code also checks if the user is selecting a new LED color, adjusting the LED brightness, or turning the LEDs on or off. If the user is selecting a new LED color, the code cycles through the color palette and updates the LED colors. If the user is adjusting the LED brightness, the code increases or decreases the brightness level. If the user is turning the LEDs on or off, the code turns the LEDs on or off accordingly.

The code includes several helper functions, including setting the LED colors based on the current color index and brightness level, and updating the LED colors when a new color is selected. The code also includes a global array of colorPalette that stores the available LED colors, and a boolean variable called ledsOn that tracks whether the LEDs are currently on or off.

Overall, this code provides a framework for a basic gamepad that includes input and output components. The code can be modified and extended to include additional buttons, sensors, and other peripherals.
