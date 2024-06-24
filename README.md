# Smart AI Bicycle Mobile App

## Overview
The Smart AI Bicycle Mobile App is designed to enhance the biking experience by providing real-time ride tracking, AI-based route suggestions, fitness tracking, maintenance alerts, social sharing, and weather updates. The app is developed in Java for Android using Firebase for user authentication, Google Maps API for location services, and various other libraries for additional functionalities.

## Features
1. **User Authentication**
    - Sign up and login using Firebase.
    - Integration with social media accounts.

2. **Ride Tracking**
    - GPS-based real-time ride tracking.
    - Display real-time stats such as speed, distance, and time.

3. **AI-based Route Suggestions**
    - Recommend routes based on user preferences and historical data.

4. **Fitness Tracking**
    - Track calories burned and heart rate (if connected to a heart rate monitor).

5. **Maintenance Alerts**
    - Notify users about bicycle maintenance based on usage.

6. **Social Sharing**
    - Share rides on social media.

7. **Weather Updates**
    - Provide weather forecasts for planned routes.

## Architecture
- **MVC (Model-View-Controller)** or **MVVM (Model-View-ViewModel)** pattern.
- **Firebase** for user authentication, database, and cloud storage.
- **Google Maps API** for route and location services.
- **ML Kit** or custom AI models for route recommendations.

## Project Structure
```
app/
├── java/
│   └── com.smartbicycle.smartbicycle/
│       ├── activities/
│       │   ├── LoginActivity.java
│       │   ├── MainActivity.java
│       ├── fragments/
│       │   ├── TrackingFragment.java
│       │   ├── ProfileFragment.java
│       ├── models/
│       │   ├── User.java
│       │   ├── Ride.java
│       ├── utils/
│       │   ├── FirebaseUtils.java
│       │   ├── RouteUtils.java
├── res/
│   ├── layout/
│   │   ├── activity_login.xml
│   │   ├── activity_main.xml
│   │   ├── fragment_tracking.xml
│   │   ├── fragment_profile.xml
│   ├── values/
│   │   ├── strings.xml
│   │   ├── styles.xml
```

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/samwelnyandoro/SmartBicycle.git
   cd SmartBicycle
   ```

2. **Open the Project in Android Studio**
    - Open Android Studio.
    - Select "Open an existing Android Studio project".
    - Navigate to the cloned repository and open it.

3. **Add Firebase to Your Project**
    - Go to the [Firebase Console](https://console.firebase.google.com/).
    - Create a new project or select an existing one.
    - Add an Android app to your Firebase project.
    - Follow the instructions to download the `google-services.json` file and place it in the `app` directory.
    - Add the Firebase SDK to your `build.gradle` files.

4. **Configure Google Maps API**
    - Go to the [Google Cloud Console](https://console.cloud.google.com/).
    - Create a new project or select an existing one.
    - Enable the Maps SDK for Android.
    - Obtain an API key and add it to your `AndroidManifest.xml`:
      ```xml
      <meta-data
          android:name="com.google.android.geo.API_KEY"
          android:value="YOUR_API_KEY"/>
      ```

5. **Run the App**
    - Connect an Android device or start an emulator.
    - Run the app from Android Studio.

## Dependencies
```gradle
// Firebase
implementation 'com.google.firebase:firebase-auth:21.0.1'
implementation 'com.google.firebase:firebase-database:20.0.3'

// Google Maps
implementation 'com.google.android.gms:play-services-maps:18.0.2'
implementation 'com.google.android.gms:play-services-location:21.0.1'

// Google Fit
implementation 'com.google.android.gms:play-services-fitness:21.0.1'
```

## Contributing
Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are warmly welcome.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further assistance. Happy biking!
