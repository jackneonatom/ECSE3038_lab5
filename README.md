README for the Arduino Code

Expected Behavior of Each Function:
1. setup():
   - Initializes the 20x4 I2C LCD display and sets up the backlight.
   - Initiates serial communication at a baud rate of 9600.
   - Attempts to connect to a WiFi network using the provided credentials (ssid and password).
   - Prints the status of the WiFi connection and the local IP address once connected.

2. loop():
   - Initializes an HTTPClient object.
   - Makes an HTTP GET request to the specified endpoint using the provided API key in the header.
   - Checks the HTTP response code and proceeds if the code is greater than 0.
   - Retrieves the response body as a string and prints it to the serial monitor.
   - Deserializes the JSON response into a JSON document.
   - Extracts the values of "line_1" and "line_2" from the JSON document.
   - Displays "line_1" and "line_2" on the LCD display at the specified positions.
   - If the HTTP response code is not greater than 0, it prints an error code to the serial monitor.
   - Frees the resources used by the HTTPClient.

Reason for Writing the Code:
The code was created to demonstrate the integration of Arduino with WiFi connectivity, HTTP requests, JSON parsing, and the display of retrieved data on an I2C LCD. It serves as a practical example for IoT projects, data visualization applications, and educational purposes, showcasing how to fetch, process, and display data from a web API.

Riddle:
Why did the scarecrow win an award? Because he was outstanding in his field!
