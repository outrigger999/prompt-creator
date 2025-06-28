## Codebase Summary

### Key Components and Their Interactions
- `pb4.py`: Main application file, containing the core logic and UI for the prompt building tool. It is composed of several classes:
    - `DataManager`: Handles loading and saving data to CSV files.
    - `ElementCreator`: Renders the UI for creating new prompt elements.
    - `ElementEditor`: Renders the UI for editing existing prompt elements.
    - `PromptBuilder`: Renders the UI for building prompts from the elements.
    - `PromptBrowser`: Renders the UI for browsing saved prompts.
- `prompt_elements.csv`: Data file used to populate UI elements.
- `prompt_history.csv`: Data file for storing user's previous prompts.

### Data Flow
- The application reads from `prompt_elements.csv` to display options in the UI.
- User interactions and generated prompts are saved to `prompt_history.csv`.

### External Dependencies
- `streamlit`: Used for creating the web application and UI.
- `pandas`: Used for data manipulation and management.

### Recent Significant Changes
- Implemented a fix to clear the input fields on the mail screen after a new element is created.
- Used Streamlit's `session_state` and a callback function to handle the state of the input fields.