# 🍃 DishCraft — AI Recipe Generator

**Turn everyday ingredients into personalized recipes with AI.**

DishCraft is a web-based AI recipe generator built with Python, Gradio, and the Google Gemini API. It helps users discover meal ideas using ingredients they already have, while considering their dietary preferences and available cooking time.
🚀 **Live Demo:** https://dishcraft-ai-recipe-generator.onrender.com
## ✨ Features

- **AI-Powered Recipe Generation:** Generates recipes from user-provided ingredients using Google Gemini.
- **Meal Customization:** Supports breakfast, lunch, dinner, and snacks.
- **Dietary Preferences:** Includes vegetarian, vegan, high-protein, and unrestricted options.
- **Cooking Time Preferences:** Allows users to request recipes within 15, 30, or 60 minutes.
- **Structured Recipe Output:** Displays ingredients, preparation time, cooking instructions, chef's tips, and ingredient substitutions.
- **Responsive Web Interface:** Provides a clean, light-themed interface using Gradio and custom CSS.
- **Input Validation & Error Handling:** Handles empty input and API failures with user-friendly messages.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Application logic |
| Google Gemini API | AI-powered recipe generation |
| Gradio | Interactive web interface |
| HTML & CSS | Interface styling |
| python-dotenv | Environment variable management |

## ⚙️ How It Works

1. The user enters available ingredients.
2. The user selects a meal type, dietary preference, and maximum cooking time.
3. The application builds a structured prompt based on these preferences.
4. The prompt is sent to the Google Gemini model through its API.
5. The generated recipe is displayed in a readable format.

## 🚀 Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/mariambanyounis/DishCraft-AI-Recipe-Generator.git
cd DishCraft-AI-Recipe-Generator
```

**2. Install dependencies**

```bash
pip install -r requirements.txt
```

**3. Configure your Gemini API key**

Create a `.env` file in the project folder:

```env
GEMINI_API_KEY=your_api_key_here
```

**Never commit your API key or `.env` file to GitHub.**

**4. Run the application**

```bash
python app.py
```

Open the local URL shown in the terminal.

## 🔐 Security

The Gemini API key is loaded from an environment variable and is not hardcoded in the application. The `.env` file is excluded from version control.

## 📌 Project Notes

- DishCraft integrates a pre-trained Gemini model; it does not train a new AI model.
- Recipe generation depends on the availability of the Gemini API.
- AI-generated recipes and cooking times are suggestions and should be reviewed for accuracy, allergens, and food safety.

## 🔮 Future Improvements

- Recipe history and favorites
- Multiple recipe suggestions
- Ingredient-based shopping lists
- Multilingual support

---

**Built with Python, Gradio, and Google Gemini API.**
