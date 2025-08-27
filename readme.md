# V.I.S.I.O.N - A Voice-Controlled AI Assistant

V.I.S.I.O.N is a voice-controlled AI assistant built in Python. It uses the OpenAI API for intelligent conversation and can perform various tasks based on voice commands.

## Features

-   **Conversational AI:** Have a natural conversation with the assistant.
-   **Voice Commands:** Control the assistant using your voice.
-   **Web Search:** Open websites like Google, YouTube, and Wikipedia.
-   **Time Telling:** Get the current time.
-   **Music Playback:** Play a local music file.
-   **Customizable:** Easily add your own custom commands and applications.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/sukeerthilangu08/V.I.S.I.O.N.git
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd V.I.S.I.O.N
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1.  **Get an OpenAI API Key:**
    -   Go to [https://beta.openai.com/account/api-keys](https://beta.openai.com/account/api-keys) and get your API key.

2.  **Add the API Key to the configuration file:**
    -   Open the `config.py` file.
    -   Replace `"YOUR_API_KEY"` with your actual OpenAI API key.

## Usage

Run the following command to start the assistant:

```bash
python vision.py
```

You can then start giving voice commands to the assistant.

## Customization

You can add your own custom commands to the `vision.py` file.

### Music Playback

To play a specific music file, open `vision.py` and change the `musicPath` variable to the path of your music file.

### Custom Applications

To add a custom application launcher, open `vision.py` and add a new `if` block in the main loop, like this:

```python
if "open my app".lower() in query.lower():
    os.system(f"open /Applications/MyApp.app")
    continue
```
