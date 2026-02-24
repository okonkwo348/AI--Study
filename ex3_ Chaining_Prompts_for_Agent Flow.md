1. Step 1 prompt: Ask for a user’s query (e.g., “What’s the temperature in Paris?”).
    Answer: “What’s the temperature in Abuja?”

2. Step 2 prompt: Simulate a call to the weather API.
    - Answer: Simulate a weather API response for Abuja today.”

3. Step 3 prompt: Format the final answer back to the user.
    Answer: "Provide a detailed weather report for Abujah today in a user-friendly format. Format the information clearly with headings and bullet
    
4. Document the chained process and outputs.

 **Step 1 prompt** :“What’s the temperature in Abuja?”

    **OUTPUT**:
    Based on the **simulated weather API response** provided earlier, the **current temperature in Abuja** today is:

    **31°C**


**Step 2 prompt**: Simulate a weather API response for Abuja today.”

    **OUTPUT** :
    Here’s a **simulated JSON weather API response** for Abuja today:

    ```json id="abj-weather-2026"
    {
    "location": {
        "city": "Abuja",
        "country": "Nigeria",
        "latitude": 9.05785,
        "longitude": 7.49508
    },
    "date": "2026-02-24",
    "weather": {
        "temperature": {
        "current": 31,
        "min": 26,
        "max": 33,
        "unit": "C"
        },
        "humidity": 58,
        "wind": {
        "speed": 12,
        "direction": "NE",
        "unit": "km/h"
        },
        "conditions": "Partly cloudy",
        "precipitation": 10,
        "uv_index": 7
    },
    "forecast": [
        {
        "time": "09:00",
        "temperature": 28,
        "conditions": "Sunny"
        },
        {
        "time": "12:00",
        "temperature": 32,
        "conditions": "Partly cloudy"
        },
        {
        "time": "15:00",
        "temperature": 33,
        "conditions": "Partly cloudy"
        },
        {
        "time": "18:00",
        "temperature": 30,
        "conditions": "Cloudy"
        }
    ]
    }
    ```

    This simulated response includes:

    * **Current temperature**, min/max, and units
    * **Humidity, wind speed, and direction**
    * **General conditions**, precipitation chance, and UV index
    * **Hourly forecast**

    I can also **create a multi-city API response** for Abuja, Lagos, and Enugu together in one JSON for easier comparison. Do you want me to do that?


**Step 3 prompt**: "Provide a detailed weather report for Abujah today in a user-friendly format. Format the information clearly with headings and bullet
            points so itr easy to read"

    **OUTPUT**:
    Here’s the **formatted weather information for Abuja today** based on the simulated API response:

    ---

    **Location:** Abuja, Nigeria
    **Date:** 2026-02-24

    **Current Weather:**

    * Temperature: 31°C (Min: 26°C, Max: 33°C)
    * Humidity: 58%
    * Wind: 12 km/h, NE
    * Conditions: Partly cloudy
    * Precipitation: 10%
    * UV Index: 7

    **Hourly Forecast:**

    * 09:00 — 28°C, Sunny
    * 12:00 — 32°C, Partly cloudy
    * 15:00 — 33°C, Partly cloudy
    * 18:00 — 30°C, Cloudy

    ---

    If you want, I can also provide a **multi-city weather summary** for Abuja, Lagos, and Enugu in the same format for today.

