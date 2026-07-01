================================================================================
                              WEATHER APP
================================================================================

A simple, elegant weather application that fetches real-time weather data using 
the OpenWeatherMap API. Built with HTML, CSS, and JavaScript.

================================================================================
FEATURES
================================================================================

  * Real-time Weather Data - Fetches current weather information for any city 
    worldwide
  * Temperature Display - Shows temperature in Celsius (�C)
  * Weather Conditions - Displays weather description and corresponding emoji
  * Humidity Information - Shows humidity percentage
  * Responsive Design - Optimized for both desktop and mobile devices
  * Error Handling - User-friendly error messages for invalid inputs or API 
    issues
  * Modern UI - Clean interface with gradient background and smooth animations

================================================================================
PREREQUISITES
================================================================================

  * A modern web browser (Chrome, Firefox, Safari, Edge)
  * OpenWeatherMap API key (free tier available)

================================================================================
INSTALLATION
================================================================================

  1. Clone the repository
     git clone https://github.com/Macpernamcfarna/weather-app.git
     cd weather-app

  2. Get an API Key
     - Sign up at OpenWeatherMap (https://openweathermap.org/api)
     - Get your free API key from the dashboard

  3. Configure the API Key
     - Open weather.js
     - Replace the apiKey variable with your key:

  4. Open the Application
     - Simply open weather.html in your browser
     - Or use a live server extension in VS Code

================================================================================
PROJECT STRUCTURE
================================================================================

  weather-app/
  ├── weather.html      # Main HTML structure
  ├── weather.css       # Styles and responsive design
  ├── weather.js        # Application logic and API integration
  └── README.txt        # Project documentation

================================================================================
HOW TO USE
================================================================================

  1. Enter a city name in the input field
  2. Click the "Get Weather" button or press Enter
  3. View the weather information displayed on the card:
     - City name
     - Current temperature
     - Humidity percentage
     - Weather description
     - Weather emoji

================================================================================
WEATHER EMOJIS
================================================================================

  Thunderstorm          �
  Drizzle/Rain          �
  Snow                  ❄️
  Mist/Fog              �
  Clear Sky             ☀️
  Clouds                ⛅
  Unknown               ❓

================================================================================
RESPONSIVE DESIGN
================================================================================

  The application is fully responsive and adapts to different screen sizes:

  * Desktop - Full-sized input, button, and card display
  * Mobile/Tablet - Adjusted sizing and layout for smaller screens

================================================================================
CUSTOMIZATION
================================================================================

  Change Temperature Unit
  -----------------------
  To display temperature in Fahrenheit, modify the displayWeatherInfo function:

  // Replace the Celsius calculation with:
  const tempF = ((temp - 273.15) * 9/5 + 32).toFixed(1);
  tempDisplay.textContent = `${tempF}�F`;

  Add More Weather Details
  ------------------------
  You can easily add more weather data from the API response:

  const { 
      name: city,
      main: { temp, humidity, pressure, feels_like },
      wind: { speed },
      weather: [{ description, id }]
  } = data;

  Modify Styling
  --------------
  * Background colors can be changed in weather.css
  * Card colors and shadows are easily customizable
  * Button hover effects can be adjusted

================================================================================
COMMON ISSUES
================================================================================

  "Could not fetch weather data"
  ------------------------------
  * Check your internet connection
  * Verify your API key is correct
  * Ensure the city name is spelled correctly
  * Check if you've exceeded the API rate limit

  "Please enter a city"
  ---------------------
  * The input field cannot be empty
  * Enter a valid city name

  API Key Not Working
  -------------------
  * Make sure you've replaced the placeholder API key
  * Check if your API key is activated
  * Verify you're using the correct API endpoint

================================================================================
SECURITY NOTE
================================================================================

  IMPORTANT: For production use, move the API key to a backend server. Exposing 
  API keys in client-side code is a security risk.

================================================================================
FUTURE ENHANCEMENTS
================================================================================

  [ ] Add 5-day weather forecast
  [ ] Unit toggle (Celsius/Fahrenheit)
  [ ] Geolocation support for automatic city detection
  [ ] Weather icons from OpenWeatherMap
  [ ] Dark mode toggle
  [ ] Save favorite cities
  [ ] Wind speed and pressure display
  [ ] Search suggestions/autocomplete

================================================================================
CONTRIBUTING
================================================================================

  Contributions are welcome! Feel free to:
  * Fork the repository
  * Create a feature branch
  * Submit a pull request

================================================================================
LICENSE
================================================================================

  This project is open source and available under the MIT License.

================================================================================
ACKNOWLEDGMENTS
================================================================================

  * OpenWeatherMap for providing the weather API
  * Icons and emojis for visual representation
  * All contributors and users of this project

================================================================================
CONTACT
================================================================================

  Macperna Mcfarna  - macpernamcfarna@gmail.com

  Project Link: https://github.com/Macpernamcfarna/weather-app

================================================================================
                    Made with ❤️ and JavaScript
================================================================================
