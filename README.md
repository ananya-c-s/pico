# Jarvis Voice Assistant (Wake Word + Voice Commands)

This is a simple Python demo of a voice assistant that:

1. Listens for a custom wake word ("Jarvis") using **Picovoice Porcupine**.
2. Once triggered, listens for specific voice commands using **Picovoice Rhino**.
   Note: Here we have used prebuilt .rhn files and didn't train the porcupine model as I didn't have credits. You can custom train it for a different keyword and another intent too.
3.
4. ## Features

- **Wake Word Detection**: Activates on the phrase "Jarvis".
- **Intent Recognition**: Supports custom commands via a Rhino context (`smart_lighting_windows.rhn`).
- **Cross-platform Support**: Works on systems supported by Picovoice libraries.

## Requirements

- Python 3.7+
- Dependencies:

  - `pvporcupine`
  - `pvrhino`
  - `pvrecorder`
  - `dotenv`

## Setup

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-folder>
```

2. Install dependencies:

```bash
pip install pvporcupine pvrhino pvrecorder python-dotenv
```

3. Set your **Picovoice Access Key**:
   Create a `.env` file in the root directory:

```
ACCESS_KEY=your-picovoice-access-key
```

4. Ensure the Rhino context file is available at:

```
models/smart_lighting_windows.rhn
```

## Running the Assistant

```bash
python your_script_name.py
```

## Usage

- Say **"Jarvis"** to activate.
- Then say a command like **"turn on the lights"**.
- The system will print the recognized intent and slots.

## Working Code Video

- Link: https://youtu.be/N0AUzgKbhXY

## License

This project is for educational/demonstration purposes. Ensure you comply with Picovoice's licensing for Porcupine and Rhino.

---
