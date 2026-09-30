# Weather App

## Overview

This project is a React weather application built with Vite. Users can search for a city and view its current weather conditions, including temperature, weather description, and wind speed. The app also displays a loading indicator while retrieving weather data and an error message when a city cannot be found.

## Project Purpose

The goal of this project is to build a browser-based weather app while practicing React components, state management, API requests, and CSS styling.

## Features

- Searches for a city when the user presses Enter
- Retrieves current weather data from the OpenWeatherMap API
- Displays the city, country, current date, temperature in Celsius, weather description, and wind speed
- Shows a loading indicator while a request is in progress
- Displays an error message when the requested city is unavailable

## Project Setup

The project uses Vite to run and build the React application. React and the required supporting packages are listed in `package.json`.

To install dependencies and start the development server:

1. Run `npm install`.
2. Run `npm run dev`.
3. Open the local URL printed in the terminal.

To create a production build, run `npm run build`.

## Application Structure

- `App.jsx` contains the weather search interface, API request, and weather display.
- `App.css` contains the application styles.
- `src/main.jsx` mounts the React application and renders `App.jsx`.
- `index.html` provides the page entry point and the `root` element used by React.
- `package.json` defines the project dependencies and available scripts.

## How the App Works

1. The user enters a city name.
2. Pressing Enter starts a request to the OpenWeatherMap current weather API.
3. The app displays a loading indicator while the request is in progress.
4. If the request succeeds, the app displays the returned weather information.
5. If the city cannot be found or the request fails, the app displays an error message.

## User Experience

The interface presents search and weather information in a centered layout. Weather details appear after a successful search, while loading and error states provide feedback during and after a request.

## Conclusion

This project brings together React, API integration, and CSS to create a functional weather application. It demonstrates how a user search can retrieve and display live weather data in a browser-based interface.