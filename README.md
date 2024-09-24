# Ollama Termux Installer

Ollama allows you to run local language models like Llama 2 and other powerful AI models without needing to rely on cloud services. This project helps you install Ollama on Termux for Android.

Features

Run large language models (LLMs) like Llama 2, Phi, and more locally.

Use Ollama's command-line tools to interact with models.

Install models directly and run them offline for privacy.

Full customization support with Ollama's Modelfile.


Prerequisites

Termux (You can install it from the Play Store or F-Droid).

A stable internet connection for downloading required packages and models.


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
wget https://github.com/Dev-ing-ing/ollama-termux/releases/download/v1.0.0/ollama-installer.sh && bash ollama-installer.sh
```


This script installs all dependencies, clones the Ollama repository, and builds Ollama from source. After successful installation, the Ollama binary will be available globally in your Termux environment.

Usage

After installation, you can run Ollama to interact with models:

first before doing any thing start a new session in termux other then the main one and type(this process needs to be repeated everytime termux is restarted:

```sh
ollama serve
```

go back in the main session (session 1) and now yo van use ollama

List available models:

```sh
ollama list
```
Download and use a model (e.g., Llama2):
```sh
ollama pull llama2
```
```sh
ollama run llama2
```

Customize models: You can create custom models by editing the Modelfile and setting parameters like temperature and system messages.


Model Library

Ollama supports various models like:

Llama2

Phi

Code Llama

Lama3

tinylama

More models can be found on the official Ollama model library.

Troubleshooting

If the installation process fails, rerun the installer by following the same steps. This script ensures that all steps are retried until successful.
