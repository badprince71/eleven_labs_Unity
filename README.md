
## Introduction

This Unity project is designed to integrate Elevenlabs API with streaming functionality via WebSocket. The project includes a WebSocket server that receives tokenized messages from the client and forwards them to the Elevenlabs API for processing.

Currently, we are using MPV (Media Player) instead of Unity's integrated `AudioSource` for audio playback. This is a temporary setup for testing purposes, as the project is still in development. The final version will integrate audio playback using Unity's `AudioSource` component, providing a more seamless and native audio experience within Unity.

### Unity Version

This project is developed using **Unity 2023.2.8f1**. Ensure that you are using this version or a compatible one to avoid any issues with compatibility.

### Required Plugins

To successfully run this project, you need to have the following plugins:

1. **websocket-sharp**:
   - This plugin is used to manage WebSocket connections within Unity. 
   - You can download it from its GitHub repository: [websocket-sharp](https://github.com/sta/websocket-sharp).

2. **Newtonsoft.Json**:
   - This plugin is used for JSON serialization and deserialization within the project.
   - You can download it via the Unity Asset Store or directly from the [official Newtonsoft.Json GitHub repository](https://github.com/JamesNK/Newtonsoft.Json).

### Download and Configure MPV (Windows)

To set up MPV on Windows, follow these steps:

1. **Download MPV**:
   - Go to the official MPV website: [https://mpv.io/installation/](https://mpv.io/installation/)
   - Scroll down to the **Windows** section and download the latest build. You can use the [SourceForge](https://sourceforge.net/projects/mpv-player-windows/files/) link provided on the site.

2. **Extract MPV**:
   - Extract the downloaded zip file to a location of your choice, such as `C:\Program Files\mpv`.

3. **Add MPV to Your System Path**:
   - Open the Start Menu, search for "Environment Variables," and open the "Edit the system environment variables" option.
   - In the System Properties window, click on the "Environment Variables" button.
   - Under "System variables," find and select the `Path` variable, then click "Edit."
   - Click "New" and add the path to the folder where you extracted MPV (e.g., `C:\Program Files\mpv`).
   - Click "OK" to close all the windows.

4. **Test MPV Installation**:
   - Open a Command Prompt and type `mpv --version` to verify the installation. You should see MPV's version information.

After setting up MPV, the project should be able to use it for audio playback during testing.

Follow the instructions below to set up and configure the project, including setting up API keys, WebSocket server details, and handling message streaming.
