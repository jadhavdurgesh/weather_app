# weather_app_tutorial

🌦️ Weather App

This is a Flutter-based Weather App that fetches and displays the current weather information for a user’s current location. The app uses OpenWeather API to retrieve weather data and the Geolocator package to fetch the user’s current location.

📱 Features

	•	Displays current weather (temperature, wind speed, humidity, etc.) for the user’s current location.
	•	Shows weather details like:
	•	Location name
	•	Current temperature
	•	Max/Min temperatures
	•	Weather description and icon
	•	Wind speed
	•	Humidity level
	•	Automatically fetches location-based weather using the device’s GPS.

🛠️ Technologies Used

	•	Flutter: Cross-platform framework for building Android and iOS apps.
	•	OpenWeather API: Provides real-time weather information based on location.
	•	Geolocator: Flutter package for accessing device location (GPS).
	•	intl: For formatting date and time.

🏗️ Setup Instructions

1. Prerequisites

	•	Flutter SDK installed (installation guide).
	•	An API key from OpenWeather.
	•	Device or emulator with location services enabled.

2. Clone the Repository

git clone https://github.com/your-username/weather-app.git
cd weather-app

3. Install Dependencies

Run the following command to install the required Flutter packages:

flutter pub get

4. OpenWeather API Key

	•	Get your API key from the OpenWeather API.
	•	Create a file called consts.dart in the lib/ directory.
	•	Add the following content, replacing YOUR_API_KEY with your actual API key:

const String OPENWEATHER_API_KEY = 'YOUR_API_KEY';

5. Location Permissions

For Android:

	•	In android/app/src/main/AndroidManifest.xml, add the following permissions:

<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>

For iOS:

	•	In ios/Runner/Info.plist, add the following entries:

<key>NSLocationWhenInUseUsageDescription</key>
<string>This app needs access to your location to display the weather for your area.</string>
<key>NSLocationAlwaysUsageDescription</key>
<string>This app needs access to your location to display the weather for your area.</string>

6. Run the App

Use the following command to run the app on your connected device or emulator:

flutter run

📂 Project Structure

.
├── lib
│   ├── main.dart        # Main entry point of the app
│   ├── consts.dart      # API Key and constants (to be created manually)
│   └── home_page.dart   # Main page displaying the weather
├── android              # Android-specific configurations
├── ios                  # iOS-specific configurations
└── pubspec.yaml         # Flutter and Dart dependencies

🌍 APIs Used

	•	OpenWeather API: Provides current weather data.
	•	Geolocator: Provides the user’s current GPS location.

🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

📝 License

This project is licensed under the MIT License - see the LICENSE file for details.


https://github.com/user-attachments/assets/2b8caae2-733d-43cf-a078-98fe61684c10




