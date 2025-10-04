# Copilot Instructions for Voice Notepad

## Project Overview
Voice Notepad is a Python-based GUI application for speech-to-text note-taking. It supports both Windows and Linux, with platform-specific code in the respective folders. The app provides voice recording, text export, and reset functionality via a simple GUI.

## Architecture & Key Components
- **Platform Separation:**
  - `Windows/voicenote.py` and `Linux/voicenote.py` are the main entry points for each OS. Each implements the GUI and core logic for its platform.
  - Images and icons are stored in `Windows/` and `Linux/` folders for platform-specific UI.
- **GUI:**
  - Built with Python (likely Tkinter, see `voicenote.py`).
  - Three main buttons: Record (Speak), Export, Reset.
- **Speech Recognition:**
  - Uses external Python packages (see `requirements.txt`).
  - Requires `PyAudio` (manual install for Windows, see README).

## Developer Workflows
- **Installation:**
  - Install dependencies: `python3 -m pip install -r requirements.txt` (Windows) or `pip3 install -r requirements.txt` (Linux).
  - For Windows, install PyAudio manually from a `.whl` file.
- **Running the App:**
  - Windows: `python3 Windows/voicenote.py`
  - Linux: `python3 Linux/voicenote.py`
- **Exporting Notes:**
  - Use the Export button in the GUI to save notes.

## Conventions & Patterns
- **Platform-specific logic:**
  - Keep OS-specific code in the respective folders.
  - Shared assets (like `Image/VoiceNote.png`) are referenced in both versions.
- **No central tests or CI for Python code:**
  - No test scripts or test folders detected; manual testing via GUI is expected.
- **External dependencies:**
  - All required packages are listed in `requirements.txt`.
  - PyAudio must be installed manually on Windows.

## Integration Points
- **Speech-to-text:**
  - Relies on internet connectivity for speech recognition.
- **Export:**
  - Exports notes to a file via GUI (see Export button logic in `voicenote.py`).

## Examples
- To run on Windows:
  ```pwsh
  python3 Windows/voicenote.py
  ```
- To install dependencies:
  ```pwsh
  python3 -m pip install -r requirements.txt
  ```

## Key Files & Directories
- `Windows/voicenote.py` — Main app for Windows
- `Linux/voicenote.py` — Main app for Linux
- `requirements.txt` — Python dependencies
- `Image/` — Shared images

## Contribution
- Open issues or PRs for bugs, typos, or improvements.
- See README for contact and contribution details.

---
For questions about platform-specific logic or missing features, review the respective `voicenote.py` file and the README. If any section is unclear or incomplete, please provide feedback for further refinement.
