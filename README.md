# ✈️ TRIP_PILOT — AI Travel Planning Agent

## 📌 About the Project

TRIP_PILOT is an AI-powered travel planning assistant built using Python, Google Agent Development Kit (ADK), and Groq's Llama 3.3 70B model. It helps users plan their trips through conversational interactions and search for flight options based on their travel preferences.

## 🚀 Features

* 💬 Conversational AI travel assistant
* 🌍 Airport code lookup for Indian and international cities
* 📅 Travel date validation
* ✈️ One-way and round-trip flight searches
* 👥 Passenger selection
* 💺 Multiple cabin classes: Economy, Premium Economy, Business, and First Class
* 📊 Flight details including airline, departure, arrival, duration, stops, and price
* 🔗 Flight booking links for multiple platforms
* 🤖 AI-powered step-by-step travel planning

## 🛠️ Technologies Used

* Python
* Google Agent Development Kit (ADK)
* Groq API
* Llama 3.3 70B Versatile
* LiteLLM
* fast-flights

## 📂 Project Structure

```text
TRIP_PILOT/
├── agent.py
├── requirements.txt
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd TRIP_PILOT
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

Create a `requirements.txt` file containing:

```text
google-adk
litellm
fast-flights
python-dotenv
```

Install the required packages:

```bash
pip install -r requirements.txt
```

### 4. Configure the Groq API Key

Create a `.env` file in your project directory:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Get your API key from the Groq Console:

https://console.groq.com/

**Important:** Never upload your `.env` file or expose your API key on GitHub.

### 5. Run the Project

Google ADK supports running agents through its command-line interface. Depending on your project structure and ADK version, run the agent from the appropriate parent directory:

```bash
adk run TRIP_PILOT
```

To launch the ADK web interface, use:

```bash
adk web
```

Follow the terminal instructions to access the local interface.

## 🔄 How It Works

1. The AI assistant asks for the destination city.
2. It collects the departure city and travel date.
3. It validates the travel date.
4. It asks whether the journey is one-way or round-trip.
5. It collects the return date if required.
6. It asks for the number of passengers and cabin class.
7. It displays a trip summary for confirmation.
8. It searches for flights and presents available options.
9. It provides booking links for comparing flights.

## 💡 Future Improvements

* Add hotel recommendations.
* Integrate destination activity suggestions.
* Improve airport code validation.
* Enhance flight search reliability.
* Add a graphical user interface.
* Implement trip history and personalized recommendations.

## ⚠️ Limitations

* Flight prices and availability may change.
* Flight searches depend on the external `fast-flights` integration.
* Airport codes for unsupported cities may require manual verification.
* Booking links allow users to compare options; tickets are not purchased by the agent.

## 👨‍💻 Author

**Priyanshu**
