Modern Desktop Audio Player

🎶 Project Overview

This is a single-file, desktop audio player application designed with a dark, modern aesthetic. It provides essential media controls (Load, Play, Pause, Stop) and volume adjustment for local audio files. Built using Python's standard GUI library, Tkinter, and the powerful audio engine from the Pygame library, it serves as a lightweight and functional music utility.

✨ Features

Dark Mode UI: A clean, modern interface utilizing a dark theme (#1E1E1E) built with Tkinter's Themed Widgets (ttk).

Essential Media Controls: Complete functionality for loading, playing, pausing, and stopping local audio tracks.

Volume Control: An integrated slider for real-time adjustment of playback volume.

Cross-Format Support: Supports common audio file formats handled by pygame.mixer (MP3, WAV, OGG).

Non-Blocking User Feedback: Uses custom, non-disruptive message boxes for error handling and user notifications instead of standard browser/system alerts.

⚙️ Technologies/Tools Used

Technology

Purpose

Python

The core programming language for the application logic.

Tkinter

Used for creating the cross-platform desktop Graphical User Interface (GUI).

tkinter.ttk

Provides themed widgets for a more modern look and feel.

Pygame (mixer)

The dedicated library for initializing the audio engine, loading audio data, and controlling playback and volume.

os, time

Standard Python modules used for file path handling (os.path.basename) and general timing (though not fully implemented for seeking).

🛠️ Steps to Install & Run the Project

Prerequisites

You must have Python installed (version 3.6+) on your system.

Installation

The primary dependency is pygame. You can install it using pip:

pip install pygame


Running the Application

Save the Python code as a single file (e.g., audio_player.py).

Open your terminal or command prompt.

Navigate to the directory where you saved the file.

Execute the script:

python audio_player.py


A window titled "Modern Desktop Audio Player" will appear.

🧪 Instructions for Testing

Follow these steps to ensure all features of the audio player are working correctly:

Test Initialization: Confirm the application opens successfully and the status label reads: "Status: Stopped". The Play and Stop buttons should be disabled.

Test Loading: Click the Load Track button. A file dialog should open. Select a compatible audio file (e.g., a local .mp3 or .wav).

Expected Result: The track should automatically start playing. The status should change to "Status: Playing," and the Play/Pause button text should change to "⏸ Pause". The track title label should display the file's name.

Test Pause/Play: Click the ⏸ Pause button.

Expected Result: The audio should stop. The button text should change back to "▶ Play". The status should read "Status: Paused". Click "▶ Play" again, and playback should resume from where it left off.

Test Stop: Click the ■ Stop button while the track is playing or paused.

Expected Result: Audio stops, playback resets to the start. Status reads "Status: Stopped". The Play button remains enabled and ready to start from the beginning.

Test Volume: Move the Volume slider left and right during playback.

Expected Result: The loudness of the audio should decrease when moving the slider left (towards 0) and increase when moving it right (towards 100).

Test Error Handling (Optional): If possible, try loading a corrupted file or a file that is not an audio format.

Expected Result: A small, custom message box should pop up (e.g., "File Error") with a detailed error message, and the application should not crash.
