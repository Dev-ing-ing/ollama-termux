# Ollama Termux Installer
I just did rewrite the bash script, because the original didnt work for me.
Ollama allows you to run local language models like Llama 2 and other powerful AI models without needing to rely on cloud services. This project helps you install Ollama on Termux for Android.


Prerequisites

Termux (You can install it from the Play Store or F-Droid).

Installation

1. Update and upgrade Termux:

```sh
pkg update && pkg upgrade
```

2. Install required tools:

```sh
pkg install wget
```

3. Download and run the Ollama installer:

```sh
wget https://github.com/Thelucyinside/ollama-termux/releases/download/ollama-installer.sh && bash ollama-installer.sh
```


This script installs all dependencies, clones the Ollama repository, and builds Ollama from source. After successful installation, the Ollama binary will be available globally in your Termux environment.
