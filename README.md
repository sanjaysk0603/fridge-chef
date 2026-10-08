# 🍳 Fridge Chef

Fridge Chef is a Streamlit chat app that turns a photo of your fridge
(or a typed list of ingredients) into recipe ideas. Chat with the AI chef,
adjust the recipes with follow-ups like "make it vegetarian", then email
the final recipes to yourself with one click.

Built with Gemini (chat + vision) and Gmail SMTP.

## Features
- Upload a fridge photo or type your ingredients
- Detects ingredients and suggests 3 simple recipes with times and steps
- Diet preference (vegetarian, vegan, and more) chosen at onboarding
- Follow-up questions keep the conversation context
- "Email my recipes" button sends a summary to your inbox

## Run locally
1. Create and activate a virtual environment:
   `python -m venv venv`, then activate it
2. Install dependencies: `pip install -r requirements.txt`
3. Copy `.streamlit/secrets.toml.example` to `.streamlit/secrets.toml`
   and fill in your Gemini API key and Gmail App Password
4. Start the app: `python -m streamlit run app.py`

## Project structure
- `app.py` - the Streamlit app
- `prompts.py` - the AI chef's personality and prompts
- `requirements.txt` - dependencies
- `.streamlit/secrets.toml.example` - template for your keys