# Weather App

This is a Weather App built using **Kotlin** and **Jetpack Compose**, following the **MVI Clean Architecture** principles. The app uses the **Open-Meteo API** to fetch weather data and **Dagger Hilt** for dependency injection.

## Features

- **Current Weather Information:**
  - Temperature
  - Weather Type (e.g., Clear, Rainy, Snowy)
  - Atmospheric Pressure
  - Humidity Level
  - Wind Speed

- **24-Hour Weather Forecast:**
  - Displayed in a `LazyRow` with hourly updates

## Architecture

The app follows the **MVI (Model-View-Intent)** pattern within a **Clean Architecture** structure. This approach ensures that the codebase is modular, testable, and easy to maintain.

### Layers

1. **Presentation Layer**: 
   - Contains the UI components built with **Jetpack Compose**.
   - **ViewModel** interacts with the UI and the underlying domain layer.

2. **Domain Layer**:
   - Contains business logic and the app's use cases.
   - Interfaces are used to decouple this layer from the data layer.

3. **Data Layer**:
   - Responsible for fetching data from the **Open-Meteo API**.
   - Data is mapped to domain models before being passed to the domain layer.

## Technologies Used

- **Kotlin**: Programming language
- **Jetpack Compose**: UI toolkit for building native Android UI
- **Dagger Hilt**: Dependency injection framework
- **Open-Meteo API**: API for retrieving weather data
- **Retrofit**: For making network requests
- **Moshi**: JSON parser used with Retrofit

## Getting Started

### Prerequisites

- Android Studio Dolphin or higher
- Minimum SDK level 21

