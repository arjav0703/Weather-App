# Weather App - README

This is a simple weather application built using **HTML**, **CSS**, and **JavaScript**, which fetches weather data from the **OpenWeather API**. The app allows users to check the current weather for a specified city, including details like temperature, humidity, weather condition, and more.

## Features
- Get the current weather for any city.
- Responsive design suitable for mobile and desktop screens.

## Technologies Used
- **HTML**: For the structure of the application.
- **CSS**: For styling and responsive design.
- **JavaScript**: To interact with the OpenWeather API and dynamically display the weather data.
- **OpenWeather API**: Provides real-time weather data for cities worldwide.

## Setup Instructions

### Prerequisites
1. You need to have an **OpenWeather API Key** to fetch data from their API. You can get your API key by signing up on the OpenWeather website [here](https://openweathermap.org/api).

### Steps to Set Up

1. **Clone the repository:**
   ```bash
   git clone https://github.com/arjav0703/Weather-App.git
   ```

2. **Create an API Key:**
   - Go to [OpenWeather](https://openweathermap.org/api).
   - Sign up for an account and generate an API key (usually free for basic usage).

3. **Configure the API Key:**
   - Open the `script.js` file in the project directory.
   - Replace `YOUR_API_KEY` with your actual API key from OpenWeather.
     ```javascript
     const apiKey = 'YOUR_API_KEY';
     ```

4. **Open the App:**
   - Simply open the `index.html` file in your browser to start using the weather app.

### Project Structure

```
weather-app/
│
├── index.html        # Main HTML file with structure
├── style.css         # Styles for the app
├── script.js         # JavaScript for interacting with OpenWeather API
└── README.md         # This README file
```

### API Request & Responses

The app fetches data from the OpenWeather API using the following endpoint:

```
https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric
```

Where:
- `{city}` is the name of the city entered by the user.
- `{API_KEY}` is your personal OpenWeather API key.
- `units=metric` ensures that the temperature is displayed in Celsius.


## How It Works

1. The user enters a city name into the input field.
2. When the user clicks the "Search" button, the app sends a request to the OpenWeather API.
3. The app receives the weather data and updates the HTML to display the temperature, humidity, wind speed, and a short description of the weather.

## Example Usage

1. Enter a city in the input box (e.g., "New York").
2. Click the "Search" button to see the weather details.


### Customizing the App

- You can customize the appearance by editing the `style.css` file.
- You can also modify the JavaScript to include additional weather data (like sunrise, sunset, etc.) or change the layout.

## Contributing

If you'd like to contribute to the project:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-xyz`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to your branch (`git push origin feature-xyz`).
6. Create a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute it!

