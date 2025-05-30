## 🌟 Tool Calling with OpenAI GPT (Function Calling Demo) 🚀

## 📖 Overview
This project demonstrates how to implement Tool Calling (aka Function Calling) using OpenAI’s GPT-4 model with Python.
Learn how to define custom functions (tools), expose them to GPT, and let GPT call them dynamically during conversations. 🤖✨

## ⚙️ Features
🛠️ Define custom Python functions as tools

📋 Describe tool capabilities using JSON schema

🤖 Enable GPT to decide when and how to call your tools

🔄 Return real function results back to GPT for accurate answers

🌤️ Simple example: get_weather(location) function returning fake weather data

## 🧰 Requirements

📦 OpenAI Python SDK (openai)

🔑 OpenAI API key (Get it from OpenAI Platform)

## 🚀 Installation
Clone this repo or download the code:

git clone https://github.com/yourusername/tool-calling-demo.git
cd tool-calling-demo
Install dependencies:

pip install openai

## Set your OpenAI API key as an environment variable or directly in the code:

export OPENAI_API_KEY="your-api-key-here"   # Linux / macOS  
set OPENAI_API_KEY="your-api-key-here"      # Windows
Or in Python:

import openai
openai.api_key = "your-api-key-here"

## ▶️ Usage
Open tool_calling_demo.py.

Run the script:

python tool_calling_demo.py
Watch GPT ask about weather in a city, call your get_weather tool, and get a friendly response! 🌤️

## 🔍 How it works
📝 Define a Python function as a "tool" (e.g., get_weather(location))

🛠️ Define a JSON schema describing the tool and its inputs

💬 Send the tool info with your user message to GPT

🤖 GPT decides to call the tool and sends arguments

⚙️ Your script runs the function with those arguments

📤 Send the results back to GPT for a final user-friendly reply

## 💡 Example Function

def get_weather(location):
    return {
        "location": location,
        "temperature": "25°C",
        "condition": "Sunny"
    }
    
## 🤝 Contributing
Contributions welcome! Open issues or submit pull requests anytime. 🛠️✨

## 📄 License
MIT License — free and open source. 🆓
