# **Flight Delay Predictor - Weather and Flight Status Checker**

This Jupyter notebook demonstrates the creation of a simple prototype that helps users check flight statuses and determine if weather conditions might cause delays.

## **Features**
- Retrieves flight status using the **AviationStack API**.
- Fetches weather data for a specified city using the **Visual Crossing Weather API**.
- Analyzes weather conditions such as precipitation probability, wind speed, and general conditions to determine if the weather might impact flight delays.
- Displays the flight status and informs the user if bad weather conditions are likely to cause delays.

## **Prerequisites**
To run this notebook, you need to set up API keys for:
- **AviationStack API** (for retrieving flight status information)
- **Visual Crossing Weather API** (for fetching weather data)

Make sure to add these API keys to the **SECRETS** tab in Google Colab or store them securely in your environment.

## **Usage**
- Run the notebook cells in order.
- When prompted, enter:
  - A **flight number** (e.g., `DL1087`).
  
The notebook will automatically fetch the weather for both the departure and arrival cities based on the flight number.

The notebook will then display:
- The flight status (e.g., on-time, delayed).
- The current weather conditions in both the departure and arrival cities.
- Whether the flight might be affected by bad weather based on precipitation, wind speed, or weather conditions such as rain or snow.

## **Example Output**

```
Enter the flight number (e.g., DL1087): DL1087

Flight Status for DL1087: on-time
Departure City: Dubai
Arrival City: Heathrow

Weather in Dubai: Rain, Overcast
Precipitation Probability: 100.0%
Wind Speed: 15.0 mph
Bad weather detected in Dubai.
The flight is currently on time, but bad weather might cause a delay.

Weather in Heathrow: Overcast
Precipitation Probability: 30.0%
Wind Speed: 10.0 mph
```
