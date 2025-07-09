# 🎵 Groove Guru

**Audio Analysis, Music Mixing and Production Assistant Tool**

An intelligent music production assistant that analyzes audio characteristics and provides targeted mixing guidance, stem separation, MIDI conversion, and AI-powered music generation.

> **📍 Current Status**: This project is currently implemented as a **Jupyter notebook demo** with Gradio interface. Perfect for experimentation and learning!
> 
> **🔑 API Requirements**: Currently requires **Hugging Face API** (free) and **OpenAI API** (paid) for full functionality. This is a proof-of-concept phase - future versions will integrate free LLM models to eliminate costs.

## ✨ Features

### 🔍 **Comprehensive Audio Analysis**
- **36 audio features** across 5 analytical domains (musical, spectral, dynamic, harmonic-percussive, spatial)
- **Semantic mapping** that translates technical measurements into human-readable descriptions
- **Key detection** using Krumhansl-Schmuckler algorithm
- **Tempo analysis** with onset detection
- **Spectral analysis** including MFCCs, brightness, and timbral characteristics

### 🎛️ **AI-Powered Mixing Recommendations**
- **Automated mixing suggestions** with confidence scores and priority levels
- **Implementation-ready parameters** for EQ, compression, spatial processing, and effects
- **LLM-enhanced analysis** for professional mixing strategies
- **Interactive chatbot** for real-time mixing consultation

### 🎼 **Advanced Audio Processing**
- **Stem separation** using Meta's Demucs models (vocals, drums, bass, instruments)
- **MIDI conversion** with Spotify's Basic Pitch for melodic content
- **Experimental drum-to-MIDI** transcription using machine learning
- **AI music generation** with Meta's MusicGen models

### 🤖 **AI Integration**
- **Smart prompt generation** for music AI models
- **Text-to-music** and **melody-conditioned** generation
- **Feature-driven recommendations** based on actual audio analysis
- **Creative workflow** for generating complementary tracks

## 🛠️ Technology Stack

- **Audio Processing**: librosa, scipy
- **Machine Learning**: Meta Demucs, Spotify Basic Pitch, Meta MusicGen
- **AI Integration**: Large Language Models for enhanced analysis
- **Interface**: Gradio web interface (notebook-embedded)
- **Analysis**: Advanced signal processing and music information retrieval

## 📁 Project Structure

```
groove-guru/
├── notebooks/
│   └── groove_guru_demo.ipynb    ← 🎯 Main demo notebook (START HERE!)
├── assets/
│   └── demo_audio.wav               ← Demo audio files
├── docs/
│   └── Groove_Guru_Final_Project_Report.pdf  ← Technical report
├── requirements.txt
├── .env.example                     ← Environment variables template
├── .gitignore
└── README.md
```

## 🚀 Getting Started

### Quick Demo Setup
1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd groove-guru
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment** (required for full features)
   ```bash
   cp .env.example .env
   # Edit .env with your API keys:
   # - HUGGING_FACE_API_KEY (free - sign up at huggingface.co)
   # - OPENAI_API_KEY (paid - for GPT integration)
   ```

4. **Run the demo**
   ```bash
   jupyter notebook notebooks/groove_guru_demo.ipynb
   ```

5. **Start analyzing!**
   - Upload your audio file
   - Get comprehensive analysis
   - Review mixing recommendations
   - Chat with AI assistant
   - Generate stems, MIDI, or new music

### 🎯 Demo Workflow
1. **Upload Audio** → Load your track into the notebook
2. **Analyze** → Get detailed audio characteristics and visualizations
3. **Get Recommendations** → Receive AI-powered mixing suggestions
4. **Chat** → Ask questions about your mix to the AI assistant
5. **Generate** → Create stems, MIDI, or complementary music

## 📊 Analysis Domains

| Domain | Features | Description |
|--------|----------|-------------|
| **Musical** | Key, tempo, chroma | Fundamental musical properties |
| **Spectral** | MFCCs, centroid, rolloff | Frequency and timbral characteristics |
| **Dynamic** | RMS, crest factor, range | Loudness and compression analysis |
| **Harmonic-Percussive** | HPSS, tonnetz | Melodic vs rhythmic content separation |
| **Spatial** | Stereo width, correlation | Stereo field characteristics |

## 🎯 Use Cases

- **Music Producers**: Get professional mixing guidance tailored to your tracks
- **Audio Engineers**: Analyze frequency balance and dynamic characteristics
- **Musicians**: Extract MIDI from audio for further composition work
- **Content Creators**: Generate complementary music and isolated stems
- **Students**: Learn mixing principles through AI-powered explanations
- **Researchers**: Experiment with audio analysis and AI music generation

## 📈 Roadmap & Future Development

### 🔮 **Planned Features**
- [ ] **Free LLM Integration**: Implement open-source models (Llama, Mistral, etc.) to eliminate API costs
- [ ] **Offline Mode**: Full functionality without internet dependency
- [ ] **Standalone Web App**: Full Python backend with modern frontend
- [ ] **Enhanced UI**: Better visualizations and user experience
- [ ] **User Sessions**: Save and manage analysis history
- [ ] **Batch Processing**: Analyze multiple files at once
- [ ] **Plugin Integration**: DAW compatibility and real-time analysis

### 🏗️ **Technical Roadmap**
- [ ] **Priority**: Migrate from notebook to full web application
- [ ] **Key Goal**: Implement local LLM inference for privacy and cost elimination
- [ ] Add real-time audio processing capabilities
- [ ] Create REST API for third-party integrations
- [ ] Deploy to production environment with no API dependencies

## 🏗️ Architecture

The system follows a modular architecture with 9 core modules:
1. **Audio Features Analysis** - Core signal processing
2. **Semantic Mapping** - Human-readable feature interpretation
3. **Mixing Base Recommendations** - Rule-based mixing guidance
4. **Enhanced LLM Analysis & Chatbot** - AI-powered insights
5. **AI Music Generation Prompt** - Smart prompt engineering
6. **AI Music Generation** - Creative content generation
7. **Audio Stem Separation** - Track isolation
8. **MIDI Mapping** - Note transcription
9. **User Interface** - Gradio-based interaction layer

## 📋 Technical Documentation

For detailed technical information, implementation details, and methodology, see the [complete project report](docs/Groove_Guru_Final_Project_Report.pdf).

## ⚠️ Important Notes

- **Demo Version**: This is a demonstration implemented in Jupyter notebook
- **API Keys Required**: You need both Hugging Face (free) and OpenAI (paid) API keys for full functionality
- **Cost Consideration**: Currently uses paid OpenAI API - this is temporary until free LLM integration
- **Privacy**: Keep your `.env` file secure and never commit API keys
- **Audio Files**: Add your test audio to the `assets/` folder for easy access
- **Performance**: Processing time depends on audio length and available compute

### 🔑 **API Setup Guide**
1. **Hugging Face** (FREE): Sign up at [huggingface.co](https://huggingface.co) → Settings → Access Tokens
2. **OpenAI** (PAID): Get API key at [platform.openai.com](https://platform.openai.com/api-keys)
3. Add both keys to your `.env` file

## 🤝 Contributing

Contributions are welcome! Whether you want to:
- Add new audio analysis features
- Improve the UI/UX
- Integrate additional AI models
- Fix bugs or optimize performance

Please feel free to open issues or submit pull requests.

## 📧 Contact

**Arturo Javier Kolster Borges**  
*For questions, suggestions, or collaboration opportunities*

---

*🎶 Democratizing music production through intelligent audio analysis and AI-powered assistance.*

**Try it now**: Just run the notebook and start analyzing your music! 🚀
