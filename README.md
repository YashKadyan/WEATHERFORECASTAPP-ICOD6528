## TITLE:
CodTech IT Solutions Internship - Task Documentation: “WEATHER FORECAST APP” Using CSS, HTML, JAVASCRIPT.


## INTERN INFORMATION:

**Name:** Yash Sanjay Kadyan

**ID:** ICOD6528


# INTRODUCTION

In the realm of digital applications, weather forecasting occupies a pivotal role, universally recognized for its significance in planning daily activities, travel, and even long-term decision-making. The evolution from traditional weather broadcasts to digital forecasting platforms has revolutionized how individuals access and interpret weather information, offering real-time updates and personalized insights tailored to specific locations. This project aims to capitalize on the power of modern web technologies, such as JavaScript, HTML, and CSS, to develop a Weather Forecast App that provides users with a seamless and informative experience.
The transition to digital weather forecasting has enabled a wealth of features and functionalities, including interactive maps, personalized alerts, and detailed forecasts for various time intervals. Despite the availability of numerous weather applications in the market, there remains a significant opportunity to create a more intuitive, visually appealing, and comprehensive tool that caters to the diverse needs of users. This project is fueled by the vision to leverage the capabilities of JavaScript and the versatility of web technologies to deliver a superior weather forecasting experience that empowers users to make informed decisions based on accurate and up-to-date information.
Stay tuned as we embark on this journey to develop a Weather Forecast App that redefines how individuals interact with and understand weather forecasts, leveraging the latest advancements in web technology to create a dynamic and user-centric platform.


# Implementation

	JavaScript Framework: Utilize a modern JavaScript framework for building the frontend application.

	HTML/CSS: Use HTML5 and CSS3 for structuring and styling the user interface, ensuring compatibility with various web browsers.

	Responsive Design: Implement responsive design principles to ensure optimal viewing experience across desktop and mobile devices.

	User Interface Components: Utilize UI libraries for designing interactive and visually appealing components.


# CODE EXPLANATION



## HTML Structure:


div class="container": Serves as the main container for the Weather Forecast App, encompassing all elements within a structured layout.

div class="weather-input": Contains the input field for users to enter a city name and buttons for searching and accessing the user's current location.

h3: Displays the prompt instructing users to enter a city name.

input class="city-input": The text input field where users can type the name of a city for weather information.

button class="search-btn": Triggers the search action to fetch weather data for the entered city.

button class="location-btn": Initiates the process to retrieve weather data based on the user's current location.

div class="separator": Provides a visual separation between the input section and the weather data display section.

div class="weather-data": Encloses the section displaying weather information.

div class="current-weather": Contains the current weather details such as temperature, wind speed, and humidity.

div class="details": Wraps the specific weather data elements.

h2: Displays the city name and its corresponding weather condition.

h4: Displays details such as temperature in Celsius, wind speed in meters per second, and humidity percentage.

div class="days-forecast": Displays the forecast for the next four days.

h2: Indicates that the following content is the forecast for the upcoming days.

ul class="weather-cards": Contains individual cards for each day's forecast.

li class="card": Represents a single forecast card, displaying details like the date, temperature, wind speed, and humidity for a particular day.


## CSS Styling:

The CSS styles define the appearance and behavior of the Weather Forecast App, ensuring a cohesive and user-friendly interface. Here's an explanation of the key styling elements:

• Global Styles are applied fundamental settings to the entire document, including setting margins, padding, box-sizing, and font-family to ensure consistency across elements.

• Body Background sets a gradient background color (#E3F2FD) for the entire page, providing a visually pleasing backdrop for the app.

• Header Styles (h1) style the app title with a white color text, centered alignment, padding, and a background color (#5372F0) for emphasis.

• Container Styles (.container) aligns the content of the app in the center of the page, sets a gap between child elements, and provides padding for spacing.

• Weather Input Section Styles (.weather-input) defines the styling for the input section, including the width, input field styles, separator appearance, and button styles.

• Separator Styles (.weather-input .separator) specifies the appearance of the separator between the input field and the buttons, including its height, width, color, and text content ("or").

• Button Styles (.weather-input button) defines the appearance of buttons, including width, padding, cursor, color, font size, border radius, and background color. The location button (.location-btn) has a different background color (#6C757D) to distinguish it.

• Weather Data Section Styles (.weather-data) sets the width of the weather data section and its child elements.

• Current Weather Styles (.current-weather) styles the container for current weather information, including background color, padding, border-radius, and alignment.

• Weather Data Details Styles (.current-weather h2, .weather-data h4) defines the styles for headings and details within the current weather section, including font size, color, and margin.

• Forecast Cards Styles (.days-forecast, .weather-cards, .weather-cards .card) styles the forecast cards section and individual cards, including font size, padding, border radius, background color, and width. The forecast cards are arranged in a flex layout for responsiveness.

• Responsive Design (Media Queries) adjusts styles based on screen size to ensure the app remains usable and visually appealing across different devices. Styles for smaller screens include adjustments to padding, width, and layout to maintain readability and usability.

These styles collectively create a visually appealing and functional Weather Forecast App, enhancing user experience and interaction with weather data.


## JavaScript Functionality:

This JavaScript code adds dynamic functionality to the Weather Forecast App, including fetching weather data from an API, displaying current weather information, fetching and displaying weather forecast for the next 4 days, and handling user interactions such as searching for weather by city name and using the user's current location.


**Fetching Weather Data from an API:**

The code verifies if the user has entered a city name into the input field. If the field is empty, it alerts the user to input a city name.

When the user submits a city name, the application asynchronously fetches weather data from the OpenWeatherMap API using the entered city name.

If the fetch operation is successful, the application displays the current weather and forecast information for the specified city.

If there are any errors during the fetch operation, such as network issues or invalid city names, the application alerts the user to try again.

Additionally, users can opt to fetch weather data based on their current location using the geolocation API. If supported by the browser, the application fetches weather data based on the user's coordinates.

This approach ensures that the Weather Forecast App retrieves accurate and up-to-date weather information for the user's specified location, enhancing its usability and functionality.


**Displaying Current Weather Information:**

The code verifies if the user has entered a city name into the input field. If the field is empty, it alerts the user to input a city name.

When the user submits a city name, the application asynchronously fetches weather data from the OpenWeatherMap API using the entered city name.

If the fetch operation is successful, the application extracts relevant weather data such as temperature, wind speed, and humidity from the API response.

The extracted weather data is dynamically displayed in the application's interface, providing the user with the current weather information for the specified city.

If there are any errors during the fetch operation, such as network issues or invalid city names, the application alerts the user to try again.

This process ensures that the Weather Forecast App accurately retrieves and displays the current weather information for the user's specified location, enhancing its usability and providing valuable real-time data.


**Fetching and Displaying Weather Forecast for the Next 4 Days**

The application asynchronously fetches weather forecast data for the next 4 days from the OpenWeatherMap API using the entered city name.

Upon successful retrieval of forecast data, the application extracts relevant information for each of the next 4 days, including temperature, wind speed, and humidity.

The extracted forecast data is dynamically displayed in the application's interface, presenting the weather forecast for each of the next 4 days.

If there are any errors during the fetch operation, such as network issues or invalid city names, the application alerts the user to try again.

This process ensures that the Weather Forecast App provides the user with accurate and timely weather forecast information for the specified city, enhancing its functionality and usability.


**Handling User Interactions such as Searching for Weather by City Name**

The code checks if the user has entered a city name into the input field. If the field is empty, it alerts the user to input a city name before proceeding.

When the user submits a city name, the application asynchronously fetches weather data from the OpenWeatherMap API based on the entered city name.

Upon successful retrieval of weather data, the application dynamically displays the current weather information for the specified city.

Additionally, the application fetches and displays the weather forecast for the next 4 days, providing users with detailed information about upcoming weather conditions.

If there are any errors during the fetch operation, such as network issues or invalid city names, the application alerts the user to try again.

This process ensures that the Weather Forecast App allows users to easily search for weather information by city name, providing accurate and timely data for their specified location.


**Using the User's Current Location**

The application checks if the user's browser supports geolocation functionality.

If geolocation is supported, the application asynchronously retrieves the user's current position (latitude and longitude) using the navigator.geolocation.getCurrentPosition() method.

Using the obtained coordinates, the application constructs an API request to fetch weather data from the OpenWeatherMap API for the user's current location.

Upon successful retrieval of weather data, the application dynamically displays the current weather information for the user's current location.

Additionally, the application fetches and displays the weather forecast for the next 4 days, providing users with detailed information about upcoming weather conditions.

If there are any errors during the geolocation or fetch operation, such as user denial of location access or network issues, the application alerts the user to try again or provides appropriate feedback.

This process enables the Weather Forecast App to utilize the user's current location to provide accurate and relevant weather information, enhancing the user experience and convenience.


# USAGE

**Fetching Weather Data from an API:** Users enter a city name in the input field and click "Search" to fetch and display current weather information and a 4-day forecast from the OpenWeatherMap API.

**Displaying Current Weather Information:** Users input a city name and click "Search" to display current weather information and a 4-day forecast.

**Fetching and Displaying Weather Forecast for the Next 4 Days:**  After inputting a city name and clicking "Search," users view the weather forecast for the next 4 days.

**Handling User Interactions such as Searching for Weather by City Name:** Users input a city name and click "Search" to retrieve and display current weather and a 4-day forecast.

**Using the User's Current Location:** By clicking "User Current Location," users fetch and display current weather information and a 4-day forecast based on their geographical coordinates.



# CONCLUSION

In conclusion, the Weather Forecast Application efficiently provides users with accurate and timely weather information, offering both current conditions and a 4-day forecast. By utilizing modern web technologies and intuitive user interactions such as city-based searches and geolocation, the application enhances user experience and assists in planning activities effectively. With further development and user feedback integration, the Weather Forecast App has the potential to become an essential tool for individuals seeking reliable weather updates to plan their daily activities with ease and precision.

# OUTPUT

