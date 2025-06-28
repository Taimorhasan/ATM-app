# ATM-app
A simple desktop ATM simulator built with Python and PySide6. Users can enter card details, PIN, and withdrawal amount to simulate a transaction. The app features smooth UI transitions, theme switching, and API-based confirmation. It’s organized into modular screens and components for clean structure and reusability.
A modern desktop ATM simulator built with PySide6. Users can input card details, PINs, and withdrawal amounts to simulate transactions, complete with styled UI themes and error handling.

✨ Features
Card number input with live formatting

PIN input with virtual keypad

Preset & custom withdrawal amounts

API-based transaction confirmation

Animated transitions and error dialogs

Light and dark themes with a theme switcher

🏗️ Project Structure
graphql
Copy
Edit
src/
├── main.py                  # Application entry point and UI stack manager
├── test.py                 # Placeholder test script
├── api/
│   └── client.py            # Handles API requests for withdrawals
├── components/
│   ├── button.py            # Styled ATM button widget
│   └── error_dialog.py      # Custom error dialog using fade-in animation
├── screens/
│   ├── card_input.py        # Screen for card number input and validation
│   ├── pin_input.py         # Screen for secure PIN input with keypad
│   ├── amount_input.py      # Screen to select or enter withdrawal amount
│   └── confirmation.py      # Screen to confirm transaction and show status
├── styles/
│   ├── stylesheet.py        # Legacy stylesheet support
│   ├── theme.json           # Defines color themes
│   └── theme_manager.py     # Dynamically applies selected theme
├── utils/
│   └── animations.py        # Fade-in animation used in dialogs/screens
🚀 Getting Started
Requirements
Python 3.8+

PySide6

Setup
bash
Copy
Edit
# Create and activate virtual environment
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the application
python src/main.py
