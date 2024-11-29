# Weather-App
This is a simple Weather App built using Python's tkinter library for the GUI and requests library to fetch weather data from the OpenWeatherMap API.

Here's a README file for your project:

---

## Features

- Allows users to search for the current weather in a specified city.
- Displays the location, temperature (in Celsius and Fahrenheit), and general weather conditions.
- Alerts the user if the city cannot be found.

---

## Requirements

- Python 3.x
- `requests` library (install with `pip install requests`)
- An API key from [OpenWeatherMap](https://openweathermap.org/api)

---

## Setup and Usage

1. **Install Required Libraries**
   Ensure you have Python 3.x installed. Use pip to install the `requests` library:
   ```bash
   pip install requests
   ```

2. **Obtain an API Key**
   - Go to [OpenWeatherMap API](https://openweathermap.org/api).
   - Sign up or log in to get your API key.
   - Replace the placeholder `API_KEY` in the script with your actual API key.

3. **Run the Application**
   Save the script as `weather_app.py` and run it:
   ```bash
   python weather_app.py
   ```

4. **Search for Weather**
   - Enter the name of a city in the input box.
   - Click the "Search Weather" button to get the weather details.

---

## Code Explanation

- **API Integration**
  - The app uses the OpenWeatherMap API to fetch real-time weather data.
  - The `get_weather` function sends a GET request to the API and parses the response for relevant information like temperature and weather conditions.

- **Graphical User Interface**
  - Built with `tkinter`, the GUI includes an input field, buttons, and labels to display results.

- **Error Handling**
  - If the city is not found, a message box is displayed with an error.

---

## Example Output

1. Input: `Vancouver`  
   Output:  
   ```
   Location: Vancouver, CA  
   Temperature: 12.34°C, 54.21°F  
   Weather: Clear  
   ```

2. Input: Invalid city name  
   Output: Error message: `Cannot find city <city_name>`

---

## Notes

- Ensure a stable internet connection to fetch data from the API.
- Do not share your API key publicly to prevent unauthorized usage.

---

## Future Improvements

- Add more weather details like humidity, wind speed, and pressure.
- Enhance the GUI for better user experience.
- Implement a dropdown for autocomplete city suggestions.

--- 
