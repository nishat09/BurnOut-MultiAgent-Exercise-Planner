# 💪 BurnOut – Multi-Agent Exercise Planner

**BurnOut** is a smart, modular workout assistant built using **Streamlit** and **AI**. Designed to personalize fitness plans, estimate daily macronutrient needs, and guide users through efficient workouts — all within a lightweight and interactive interface.

This app leverages a **multi-agent architecture** to process user inputs, generate intelligent recommendations using large language models, and adapt dynamically to user goals and fitness levels.

---

## 🚀 Features

- 🧠 **AI-Powered Recommendations** – Generate personalized workout plans and macronutrient suggestions using OpenAI's GPT-based models.
- 👥 **User Profile Management** – Input your fitness level, goals, and preferences to receive tailored fitness advice.
- 🍽️ **Macro Calculator** – Calculate daily protein, carb, and fat needs based on your inputs and objectives.
- 🖥️ **Streamlit Interface** – Lightweight, clean UI with minimal setup and responsive layout.
- 🧱 **Modular Architecture** – Clearly separated agent files like `ai.py`, `db.py`, `logic.py`, and more, allowing for scalable improvements.

---

## 🧰 Tech Stack

| Component             | Tools & Libraries                                      |
|----------------------|--------------------------------------------------------|
| **Frontend + UI**    | Streamlit                                              |
| **AI Integration**   | OpenAI GPT API, LangChain / Langflow                   |
| **Architecture**     | Multi-agent modules (`ai.py`, `db.py`, `user.py`, etc.)|
| **Data Handling**    | DataStax (planned for advanced agent flow)             |
| **Language**         | Python 3.10+                                           |

---

## 🛠️ Getting Started (Run Locally)

### 🔧 Prerequisites

- Python 3.10 or higher
- [pip](https://pip.pypa.io/en/stable/installation/)
- OpenAI API Key (You can get one [here](https://platform.openai.com/account/api-keys))

---

### 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/BurnOut-MultiAgent-Exercise-Planner.git
   cd BurnOut-MultiAgent-Exercise-Planner
   ```

2. **Create and activate a virtual environment (optional but recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set your OpenAI API key (create a `.env` or pass as environment variable)**
   ```bash
   export OPENAI_API_KEY=your_api_key_here  # Linux/macOS
   set OPENAI_API_KEY=your_api_key_here     # Windows
   ```

5. **Run the app**
   ```bash
   streamlit run main.py
   ```

---

## 🧱 File Structure

```
├── main.py              # Entry point (Streamlit UI)
├── ai.py                # Handles AI workout & macro recommendations
├── db.py                # (Optional) Handles session/user input data
├── user.py              # Parses and validates user profiles
├── utils.py             # Helper functions
├── requirements.txt     # All dependencies
└── .env.example         # Template for API key config
```

---

## 📌 Status

🛠 This project is in active development. Upcoming features include:
- 🧭 Agent-based flow management with **LangGraph** or **DataStax Astra**
- 🧑‍⚕️ Injury recovery & workout alternates
- 📊 Progress tracking and visual feedback

---

## 📄 License

This project is released under the MIT License. Feel free to fork, contribute, and use in your own projects.

---

## 🙌 Contributions

Contributions are welcome! If you’d like to add agents, improve features, or refactor the codebase, please open an issue or submit a pull request.

