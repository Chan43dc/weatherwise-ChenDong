Before and After Examples

This document shows how I used ChatGPT to improve parts of my code during the WeatherWise project. Each example includes the original version, the AI prompt I used, the improved version, and a short explanation of why it’s better.

 Example 1: Improve error handling in API call


response = requests.get(url)
data = response.json()
Prompt to AI

“How can I handle errors if the API call fails or times out?”

After

python
Copy
Edit
try:
    response = requests.get(url, timeout=5)
    response.raise_for_status()
    data = response.json()
except requests.exceptions.RequestException as e:
    print("Error:", e)
    data = {}
Why this is better
This version prevents the program from crashing, and gives users clear feedback when a request fails.

Example 2: Improve temperature chart logic
Before

python
Copy
Edit
plt.plot(weather_data['forecast'])
Prompt to AI

“How do I plot daily max temperatures from wttr.in JSON?”

After

python
Copy
Edit
temps = [int(day['maxtempC']) for day in weather_data['weather'][:5]]
labels = [day['date'] for day in weather_data['weather'][:5]]
plt.plot(labels, temps, marker='o')
Why this is better
This version uses correct data keys, adds labels, and makes the graph readable and accurate.

Example 3: Dynamic location extraction in NLP
Before

python
Copy
Edit
location = "Perth"
Prompt to AI

“How can I detect the city name from a user's question?”

After

python
Copy
Edit
for word in question.split():
    if word.istitle():
        location = word
Why this is better
Now the program can dynamically detect city names instead of using a hardcoded value.
