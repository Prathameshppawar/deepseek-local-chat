
# DeepSeek Code Companion 🤖

An intelligent AI pair programmer with built-in debugging capabilities, powered by Ollama and LangChain.

![Demo Screenshot](./screenshot.png)

## Features ✨

- 🧠 Local AI processing via Ollama
- 🐍 Python-focused code assistance
- 🔄 Context-aware conversation
- 🚀 Real-time code debugging
- 🎨 Dark mode UI

## Prerequisites 📋

- [Ollama](https://ollama.ai/) installed and running
- Python 3.9+

## Installation ⚙️

1. **Set up Ollama**:
   ```bash
   # Install Ollama
   curl -fsSL https://ollama.ai/install.sh | sh

   # Pull desired models (e.g., Deepseek)
   ollama pull deepseek-r1:7b
   ```

2. **Clone repository**:
   ```bash
   git clone https://github.com/yourusername/deepseek-chat.git
   cd deepseek-chat
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Configuration 🛠️

The app will automatically:
- Detect installed Ollama models
- Connect to local Ollama instance (http://localhost:11434)
- Maintain conversation history

To customize:
- Edit `app.py` to modify system prompts
- Adjust temperature in `ChatOllama` initialization
- Modify CSS in the `st.markdown` section

## Usage 🚀

1. Start Ollama service:
   ```bash
   ollama serve
   ```

2. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

3. Use the sidebar to:
   - Select from detected models
   - View model capabilities
   - Monitor conversation flow

## Troubleshooting 🔧

**Common Issues**:
- "Model not found": Ensure model is pulled via Ollama
- Connection errors: Verify Ollama is running (`ollama serve`)
- UI issues: Clear browser cache or try incognito mode

## Roadmap 🗺️

- [ ] Multi-model collaboration
- [ ] Code execution sandbox
- [ ] Version control integration
- [ ] Performance metrics

## License 📄

MIT License - See [LICENSE](LICENSE) for details

