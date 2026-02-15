# OpenClaw with Ollama(Run Openclaw for free)

## 🦞 OpenClaw with Ollama (Android/Termux)

Run a powerful, local AI agent on your Android device for free using Termux, Ollama, and OpenClaw.

📋 Prerequisites
Before starting, ensure you have the following installed on your Android device:
Termux (Recommended version from F-Droid or GitHub).
Node.js (Required for OpenClaw).
A stable internet connection for the initial setup.

## Please visit for The Beginner's Guide
## Run this repo command till the networks setup commands.
Repo Link - https://github.com/AbuZar-Ansarii/Clawbot.git

🚀 Installation & Setup
Follow these steps in order to get your local environment running.

1. Install and Start Ollama
Open Termux and run the following command to install the Ollama package:

``` 
pkg install ollama
```
Start the Ollama server:
```
ollama serve
```
Note: Keep this session running. You will need to open a new Termux session for the following steps.

2. Download the Model
In a new Termux session, pull the desired model. For example:
```
ollama pull glm-5:cloud
```
Run model 
```
ollama run glm-5:cloud
```

3. Install OpenClaw
Install the OpenClaw CLI globally using npm:

```
npm install -g openclaw@latest
```
🛠️ Configuration
Run the onboarding wizard to configure your environment and install the background daemon:
```
openclaw onboard --install-daemon
```
⚡ Usage
Once configured, you can launch OpenClaw using the following commands:

Standard Launch:
```
ollama launch openclaw
```
Launch with Configuration Menu:
```
ollama launch openclaw --config
```
Openclaw Dasboard:
```
http://127.0.0.1:18789
```


💡 Troubleshooting
Memory Issues: Running LLMs on mobile can be resource-intensive. Ensure you have at least 4GB of free RAM.

Stay Awake: Use the termux-wake-lock command to prevent Android from killing the process when the screen is off.
