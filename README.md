
<div align="center">

#  Brand Voice Toner: Dynamic AI Rewriter

**🚀 Instantly rewrite any text to match your brand's voice with the power of local or cloud-based LLMs. 🚀**

![Python Version](https://img.shields.io/badge/python-3.11%2B-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Framework](https://img.shields.io/badge/framework-CustomTkinter-purple.svg)
![AI Backend](https://img.shields.io/badge/AI-Ollama-orange.svg)

</div>

The **Brand Voice Toner** is a powerful, dynamically-themed desktop application that uses Large Language Models (LLMs) to instantly rewrite any piece of text to match a specified brand voice (*Witty*, *Professional*, *Playful*). This tool ensures content creators have clean, structured content ready for any platform, from social media to WordPress.

<br/>

<p align="center">
  <!-- Replace this with a real screenshot or GIF of your application -->
  <img src="https://picsum.photos/seed/brandvoicetoner/800/450" alt="Brand Voice Toner Application Demo">
</p>

---

## ✨ Key Features

- **🎭 Dual Output:** Generates content simultaneously in two formats for ultimate flexibility:
  - **Plain Text:** Clean, unformatted text ready for any document or email.
  - **HTML Code:** Fully structured with tags (`<p>`, `<h2>`, `<ul>`) ready to paste directly into the **WordPress Classic Editor** or any other web editor.

- **🎨 Dynamic Theming:** Supports multiple color schemes ("Pink Magic," "Mystic Blue," "Warlock Green") which can be switched instantly, along with standard Dark/Light mode support.

- **☁️ Flexible Power Source:** Works equally well with two modes:
  - **Ollama Local:** Uses your PC's GPU/CPU for privacy, offline access, and speed.
  - **Ollama Cloud:** Connects to your cloud API key for greater model access without using local resources.

- **💾 Persistent Settings:** Automatically saves all user inputs, API keys, and theme preferences between sessions. Your workflow is always ready when you are.

- **🖱️ Native Control:** Includes a full right-click context menu (Cut, Copy, Paste) on all text fields for a seamless user experience.

---

## 🛠️ Getting Started

Follow these steps to get the Brand Voice Toner up and running on your local machine.

### Prerequisites

1.  **Install Python (v3.11 or v3.12 recommended)**
    - **Download:** Go to the [official Python website](https://www.python.org/downloads/) and download the latest stable version.
    - **Install:** During the installation process, **be sure to check the box that says "Add python.exe to PATH"**.

2.  **Install and Run Ollama**
    - **Install Ollama:** Download and install the application for your OS from the [Ollama website](https://ollama.com/).
    - **Download a Model:** Open your Command Prompt (CMD) or PowerShell and pull the base model required for the application:
      ```bash
      ollama pull llama3:8b
      ```
    - **Run Server:** Ensure the Ollama server application is running in the background before launching the app.

### Installation and Setup

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/your-username/brand-voice-toner.git
    cd brand-voice-toner
    ```

2.  **Create and Activate a Virtual Environment**
    ```bash
    # Create the environment
    python -m venv .venv

    # Activate the environment (Windows)
    .venv\Scripts\activate

    # On macOS/Linux, use: source .venv/bin/activate
    ```

3.  **Install Dependencies**
    With your virtual environment active, install the required packages:
    ```bash
    pip install customtkinter ollama
    ```

4.  **Configure Theme Files (Critical)**
    Ensure the two JSON files are present in the root directory of the project:
    - `master_themes.json` (defines the color themes)
    - `toner_settings.json` (stores user settings and API keys)

---

## 🚀 Running the Application

With your virtual environment active and the Ollama server running, launch the main script:

```bash
python toner_app.py
```

### Using Cloud Ollama

To switch from your local LLM to a cloud provider, simply select **Cloud Ollama** in the app's settings menu and enter your **Cloud API URL** (e.g., `https://ollama.com`) and **API Key**.

---

## 📦 Creating the Executable (.exe)

To share your tool with non-technical users, you can package it into a single executable file using **PyInstaller**.

1.  **Install PyInstaller:**
    ```bash
    pip install pyinstaller
    ```

2.  **Build the Executable:**
    Run the following command from the project's root directory:
    ```bash
    pyinstaller --onefile --windowed ^
    --name="BrandVoiceToner" ^
    --add-data "master_themes.json;." ^
    --add-data "toner_settings.json;." ^
    toner_app.py
    ```
    *Note: The `^` character is for line continuation in Windows CMD. On PowerShell, use a backtick `` ` ``, and on macOS/Linux, use a backslash `\`.*

The final executable, **`BrandVoiceToner.exe`**, will be located in the **`dist`** folder.

---

## 🤝 Contributing

Contributions are welcome! If you have ideas for new features, improvements, or bug fixes, please open an issue or submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

