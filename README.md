# SkyCast Weather

A lightweight desktop weather application built with Python and Tkinter. Search for any city to view its current weather, then save cities to a personal favorites list for quick access.

## Features

- Search current weather by city name
- View temperature, “feels like” temperature, humidity, wind speed, and conditions
- Weather icons that adapt to the current conditions
- Favorite-city list with quick selection and removal
- Clean, blue-themed Tkinter interface
- A five-day forecast-style visual panel

## Preview

The application uses data from the [OpenWeather API](https://openweathermap.org/api).

## Requirements

- Python 3.8 or newer
- An OpenWeather API key
- `requests`

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/skycast-weather.git
   cd skycast-weather
   ```

2. Install the dependency:

   ```bash
   pip install requests
   ```

3. Create an API key at [OpenWeather](https://openweathermap.org/api).

4. In `application.py`, replace the value of `API_KEY` with your own key:

   ```python
   API_KEY = "your_openweather_api_key"
   ```

5. Run the app:

   ```bash
   python application.py
   ```

## Notes

- Weather values are displayed in Celsius and wind speed is converted to km/h.
- The forecast strip is currently a visual mockup; it does not yet use forecast API data.
- Favorites are kept in memory, so they reset when the application closes.

## Security

Never commit a real API key to a public repository. If a key was already uploaded, revoke or rotate it in your OpenWeather account and replace it with a new one before publishing further changes.

## License

This project is available under the MIT License. Add a `LICENSE` file to the repository if you would like to apply it formally.
