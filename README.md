# HireScribe

Privacy-first interview transcription for recruiters. Record, transcribe, and summarize interviews with 100% local AI processing.

**Your candidate data never leaves your computer.**

---

## About HireScribe

HireScribe is a desktop application built specifically for recruiters who want to focus on conversations instead of note-taking. Unlike cloud-based solutions, all AI processing happens locally on your machine. No data leaves your device, no API keys required, no subscriptions.

Built by a recruiter, for recruiters.

---

## Key Features

### Recording & Transcription
- **One-click recording** from your microphone with built-in consent management
- **Upload existing audio** (MP3, WAV, M4A, OGG) via drag-and-drop
- **AI-powered transcription** using Whisper models running entirely on your device
- **Speaker identification** to distinguish who said what (optional)

### AI Summaries
- **Three summary formats**: Bullet points, short summary, and detailed summary
- **Customizable templates** for different interview types (screening, technical, behavioral, executive)
- **Editable summaries** to add your own notes and insights
- **Export to Markdown** for use in your ATS, notes, or team collaboration tools

### Privacy by Design
- **100% local processing**: no cloud, no external APIs
- **Works offline** after initial setup
- **GDPR-friendly**: you control where data is stored
- **No subscriptions**: one-time setup, unlimited use

---

## Platform Support

| Platform | Status | Notes |
|----------|--------|-------|
| **macOS (Apple Silicon)** | ✅ Fully Supported | M1/M2/M3/M4 Macs with GPU acceleration |
| **macOS (Intel)** | ⚠️ Limited | May work but not tested |
| **Windows** | 🚧 Coming Soon | Build ready, testing in progress |
| **Linux** | ❌ Not Available | Not planned for beta |

---

## System Requirements

### macOS (Apple Silicon)

| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| **Chip** | Apple M1 | Apple M1 or newer |
| **macOS** | 11.0 (Big Sur) | 13.0+ (Ventura or newer) |
| **RAM** | 8GB | 16GB |
| **Storage** | 4GB free | 6GB free |
| **Internet** | Required for initial setup only | |

### Processing Performance

On Apple Silicon with default settings:

| Interview Length | Processing Time |
|------------------|-----------------|
| 5-10 minutes | ~6-9 minutes |
| 15 minutes | ~15-18 minutes |
| 30 minutes | ~25-35 minutes |

Processing happens in the background, so you can keep using your computer.

---

## Download

### Latest Beta Release

**[Download HireScribe for macOS (Apple Silicon)](https://github.com/SourceBuddy-ai/HireScribe-downloads/releases/latest)**

1. Download the `.dmg` file
2. Open the DMG and drag HireScribe to Applications
3. Launch HireScribe and complete the setup wizard (~5 minutes)
4. Start recording or upload your first interview

*Note: On first launch, macOS may show a security prompt. Right-click the app and select "Open" to proceed.*

---

## How It Works

### First-Time Setup

The setup wizard guides you through:

1. **Hardware detection**: automatically configures for your Mac
2. **AI engine initialization**: built-in, no external services needed
3. **Model downloads**: one-time download of transcription (~500MB) and summarization (~2.6GB) models
4. **Ready to go**: start recording immediately

### Daily Use

1. **Record** an interview or **upload** an existing audio file
2. **Wait** for automatic transcription and summarization
3. **Review** the transcript and AI-generated summaries
4. **Edit** summaries to add your notes
5. **Export** to Markdown for your records

---

## What's Included

- **MLX Whisper**: GPU-accelerated transcription optimized for Apple Silicon
- **Ollama**: local LLM engine (bundled, no separate installation)
- **Qwen3 model**: summarization model optimized for interview analysis
- **Speaker diarization**: identify who spoke when (optional feature)

---

## Beta Program

HireScribe is currently in beta. We're looking for feedback from recruiters who:

- Use macOS with Apple Silicon (M1/M2/M3/M4)
- Record or transcribe interviews regularly
- Care about candidate data privacy

### Providing Feedback

- **In-app**: Use the feedback button (bottom right corner of app window) to report issues directly
- **GitHub**: [Open an issue](https://github.com/SourceBuddy-ai/HireScribe-downloads/issues) for bugs or feature requests

---

## FAQ

**Q: Do I need an internet connection?**  
Only for the initial setup to download AI models. After that, HireScribe works completely offline.

**Q: Where is my data stored?**  
All data stays on your Mac in `~/Library/Application Support/Hire Scribe/`. Audio files, transcripts, and summaries never leave your device.

**Q: How accurate is the transcription?**  
Whisper-based transcription achieves high accuracy for clear audio. Best results come from good microphones and minimal background noise.

**Q: Can I use this for video call recordings?**  
Yes. Record audio from your computer's microphone during calls, or upload audio exported from video conferencing platforms.

**Q: Is there a Windows version?**  
Windows support is coming soon. The build is ready and we're completing testing.

---

## Support

- **Documentation**: See the Help tab within the app
- **Issues**: [GitHub Issues](https://github.com/SourceBuddy-ai/HireScribe-downloads/issues)
- **Email**: [Contact support]

---

## License

HireScribe is proprietary software. See [EULA](link) and [Privacy Policy](link) for details.

---

**Stop taking notes. Start having conversations.**
