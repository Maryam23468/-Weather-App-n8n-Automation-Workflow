# -Weather-App-n8n-Automation-Workflow
⛅ Weather App — n8n Workflow
This is a simple and customizable Weather App built using n8n, an automation tool that fetches real-time weather data for a given city using the OpenWeatherMap API.

📌 Overview
This workflow allows you to:
Manually trigger weather data retrieval
Specify a city (e.g., Rawalpindi)
Get current:
Temperature
Weather conditions
Feels-like temperature
Humidity
Wind speed

🧩 Workflow Structure
Node	Function
When clicking ‘Execute workflow’	Manually starts the workflow.
Edit Fields	Sets the target city (e.g., Rawalpindi).
OpenWeatherMap	Calls the OpenWeatherMap API to fetch weather data.
Edit Fields1	Extracts and formats key weather metrics.

⚙️ Setup Instructions
Prerequisites
An instance of n8n (self-hosted or cloud)
A valid OpenWeatherMap API key

Configuration Steps
Import the workflow JSON into your n8n instance.
Set up credentials:
Type: OpenWeatherMap
Name: OpenWeatherMap account
Enter your API key
Edit the City value in the Edit Fields node to your preferred city.

🚀 How to Run
Go to your n8n canvas.
Open this workflow.
Click “Execute Workflow”.
You’ll receive a structured weather report.

📤 Example Output
json
Copy
Edit
{
  "Location": "Rawalpindi",
  "Temperature": "33°C",
  "Feels like": "36°C",
  "Weather": "Clouds (scattered clouds)",
  "Humidity": "55%",
  "WindSpeed": "4.6 m/s"
}
🛠️ Customization
You can:
Replace Rawalpindi with any other city (e.g., Karachi, Lahore, New York)
Add a cron trigger to fetch weather updates every morning
Extend it to send data via Email, Telegram, or Slack

🧪 Tips
Use Celsius or Fahrenheit by setting units in the API node.
Add conditional logic if you want alerts for extreme weather.

🤝 Contributions
Feel free to fork the project, submit issues, or open pull requests for enhancements!

📝 License
This project is licensed under the MIT License.

Let me know if you want this saved as a downloadable .md file or need a version in Urdu.
