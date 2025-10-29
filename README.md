Brand Voice Toner - Dynamic AI RewriterA professional desktop application designed to ensure content consistency by instantly rewriting text to perfectly match a specified brand voice (e.g., Witty, Professional, Playful). This tool allows content creators to work faster and deliver perfectly toned copy across all channels.✨ FeaturesDual Output Formats: Generates content simultaneously in two ready-to-use formats:Plain Text: Clean, unformatted text for quick use in emails or documents.HTML Code: Structured output using standard tags (<h2>, <p>, <ul>), optimized for direct paste into WordPress Classic Editor.Flexible Power Source: Supports both Ollama Local (for maximum speed and privacy using your PC's GPU/CPU) and Ollama Cloud (for access to larger, remote models).Dynamic Theming: Features multiple unique color schemes ("Pink Magic," "Warlock Green," "Mystic Blue") and standard Dark/Light mode switching.Native Usability: Includes a full right-click Cut/Copy/Paste context menu on all text fields.🚀 Getting Started (Installation)Follow these instructions to set up and run the application on your local Windows PC.1. PrerequisitesYou must have the following software installed:Python: Install Python 3.11 or 3.12 from the official website. (Ensure "Add python.exe to PATH" is checked during installation).Git: Install Git for Windows.Ollama: Install and run the Ollama application, then download a powerful model:ollama pull llama3:8b
2. Install DependenciesYou must install the project's required Python libraries:# Activate your virtual environment first (Highly Recommended)
.venv/Scripts/activate

# Install the required packages
pip install customtkinter ollama
3. Run the ApplicationExecute the main script after activating your environment:python toner_app.py
📦 Project FilesFileDescriptiontoner_app.pyThe main Python application script (entry point).master_themes.jsonJSON file defining the multiple dynamic color schemes for the application.toner_settings.jsonUser settings file for persistent inputs, API keys, and theme choices (created upon first run).index.htmlThe fully styled project documentation page (served live via GitHub Pages).⬇️ Distribution & Executable CreationTo package the tool into a single executable file (.exe) for easy sharing, you must install PyInstaller and run the following command:# Install PyInstaller first
pip install pyinstaller

# Run the final build command
pyinstaller --onefile --windowed ^
--name="BrandVoiceToner" ^
--add-data "master_themes.json;." ^
--add-data "toner_settings.json;." ^
toner_app.py
The final executable, BrandVoiceToner.exe, will be in the dist folder.🔗 Live Documentation<div align="center"><a href="https://hsinidev.github.io/Brand-Voice-Toner-AI/" target="_blank"><img src="https://www.google.com/search?q=https://img.shields.io/badge/VIEW%2520LIVE%2520DOCUMENTATION-0077A3%3Fstyle%3Dfor-the-badge%26logo%3Dgithub%26logoColor%3Dwhite" alt="View Live Documentation"></a></div>
