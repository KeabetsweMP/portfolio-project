

Weather App

This is a simple weather application that allows users to check real-time weather data based on the city they search for. It uses the OpenWeatherMap API to fetch current weather and forecast data, updating the content dynamically without needing to refresh the page.

Features

- Current Weather: Displays current temperature, weather description, and weather icons.
- *Hourly Forecast*: Shows the weather forecast for the next few hours based on the selected city.
- *Dynamic Search*: Users can input a city name and instantly get weather data for that city.
- *Real-Time Updates*: Weather information updates dynamically without reloading the page.
- *Error Handling*: Displays an error message if the city name is invalid or if the API request fails.

How It Works

1. *API Integration*:
   - The app fetches weather data using the OpenWeatherMap API.
   - Two types of API calls are made:
     - Current weather data: `api.openweathermap.org/data/2.5/weather`
     - Forecast data: `api.openweathermap.org/data/2.5/forecast`
   - Both calls use an API key to authenticate the requests.

2. *Dynamic Content*:
- When the user enters a city name and clicks the search button, the app fetches and displays the relevant weather data (temperature, description, icons).
   - The page updates without reloading, using JavaScript for client-side rendering.

3. *Interactive Features*:
   - *Search Field*: Users can type in a city name to search.
   - *Search Button*: Clicking this button triggers the API call and updates the weather information.
   - *Hourly Forecast*: Displays the weather forecast for the next several hours.

4. *Error Handling*:
   - If the city is not found or the API call fails, an error message is displayed to the user.

Setup

1. Clone the Repository

To get started, clone this repository to your local machine:

```bash
git clone https://github.com/KeabetsweMP/weather-app.git
```

2. Get an API Key

To access weather data, you need an API key from OpenWeatherMap.

- Go to [OpenWeatherMap](https://openweathermap.org/).
- Create an account and get your API key from the [API keys page](https://home.openweathermap.org/api_keys).
- Copy your API key.

3. Set Up the API Key

In the `app.js` (or similar JavaScript file), replace the placeholder `YOUR_API_KEY` with your actual API key:

```javascript
const apiKey = 'YOUR_API_KEY';  // Replace with your actual OpenWeatherMap API key
```

4. Open the Application

- Open the `index.html` file in your browser.
- The weather app should now be working, and you can start searching for weather by entering a city name.

File Structure

- `index.html`: The main HTML file containing the structure of the page.
- `style.css`: The stylesheet for the app's layout and design.
- `app.js`: The JavaScript file that handles API calls, dynamic content updates, and interactive elements.

Technologies Used

- *HTML*: Structure of the web page.
- *CSS*: Styling the web page for better appearance.
- *JavaScript*: For fetching API data, handling user input, and dynamically updating the page.

Troubleshooting

- *City not found error*: If you get an error that says the city is not found, make sure the city name is correct and spelled properly.
- *No data displayed*: Ensure your API key is correctly set up and that you are connected to the internet.
- *API Limitations*: If you're getting an API limit error, it may be because the free tier of OpenWeatherMap has reached its daily request limit.
