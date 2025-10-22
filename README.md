# 💻 Code Converter (Streamlit)

A modern, interactive Streamlit app to simulate converting code between languages. It supports file upload, manual input, conversion preview, history, a copy/download toolbar, and an "Ask AI" helper placeholder.

## Features
- From/To language selectors (Python, Java, C++, JavaScript)
- Prompt field with placeholder
- Drag-and-drop file uploader that populates the input area
- Input and Output code areas with syntax highlighting
- Convert button with spinner and success/error messages
- Copy to clipboard and Download actions
- "Ask AI" expander with chat-like UI (placeholder)
- Collapsible History stored in session_state
- Sidebar with theme toggle (Light/Dark) and app info
- Custom CSS for rounded corners, soft shadows, and hover effects

## Quickstart

1) Install dependencies

```bash
pip install -r requirements.txt
```

2) Run the app

```bash
streamlit run app.py
```

3) Open the browser URL shown in the terminal (typically `http://localhost:8501`).

## Project Structure

```
.
├── app.py              # Streamlit application
├── requirements.txt    # Python dependencies
└── README.md
```

## Notes
- The conversion is simulated; integrate a backend model/API in `convert_code_placeholder` to produce real translations.
- History persists only for the current Streamlit session by default.
- Copy uses the browser clipboard API; some environments may require HTTPS or user gestures.
