# IRIS Vision

A single-file Python camera assistant for Android and Pydroid 3, built with Flask and Google Gemini. HTML, CSS and JavaScript are embedded in `main.py`; no Kivy is needed.

## Run on your phone

1. Install Pydroid 3 and open its terminal.
2. Install dependencies: `pip install -U flask google-genai`.
3. Obtain a new private API key from Google AI Studio. Replace the placeholder in your local `main.py`. Never upload or commit your actual key.
4. Run `python main.py`.
5. Open **http://localhost:5000** in Chrome on the same phone and allow camera access. Keep Pydroid running.
6. Tap **Start**, hold steady for five seconds, or tap **Capture**. Use **Rescan**, **Camera ↻**, **Pause** and **Copy** as needed.

Captured JPEG photos are sent to Google Gemini for analysis. Internet and Gemini API access/quota are required. The live preview stays on your device. The server listens only on localhost. The configured model is `gemini-3-flash-preview`; availability depends on your Google AI Studio account.

The supplied keyword line outside the HTML string was removed to correct a Python syntax error. The supplied private key was replaced with a placeholder.
