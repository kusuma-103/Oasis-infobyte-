import requests
def get_weather(api_key, location):
    # URL for the OpenWeatherMap API
    url = f"http://api.openweathermap.org/data/2.5/weather?q={location}&appid={api_key}&units=metric"
    
    # Send a request to the OpenWeatherMap API
    response = requests.get(url)
    
    # Check if the request was successful
    if response.status_code == 200:
        data = response.json()
        
        # Extract relevant information
        city = data['name']
        temperature = data['main']['temp']
        humidity = data['main']['humidity']
        weather_description = data['weather'][0]['description']
        
        # Display the weather information
        print(f"Weather in {city}:")
        print(f"Temperature: {temperature}°C")
        print(f"Humidity: {humidity}%")
        print(f"Conditions: {weather_description.capitalize()}")
    else:
        print("Error: Could not retrieve weather data. Please check the location or your API key.")

def main():
    # Replace with your OpenWeatherMap API key
    api_key = "42000da9c0aa48cb4ca2c4b424f86edb"
    
    # Get user input for location
    location = input("Enter a city name or ZIP code: ")
    
    # Fetch and display weather data
    get_weather(api_key, location)

if __name__ == "__main__":
    main()

