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
- **Upload existing audio** (MP3, WAV, M4A, OGG, FLAC, WEBM, MP4) via drag-and-drop
- **AI-powered transcription** using Whisper models running entirely on your device
- **Speaker identification** to distinguish who said what (optional, macOS only)

### AI Summaries
- **Three summary formats**: Bullets (6–8 key takeaways), Short (3–4 sentence executive summary), and Medium (detailed summary organized by topic)
- **11 built-in templates**: General Interview, Technical Interview, Behavioral Interview, Sales Interview, Executive Interview, Phone Screen, Hiring Manager Intake, Stakeholder Meeting, Client Discovery Call, Debrief Call, and Voice Memo
- **Custom templates** — build your own with any sections you need
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
| **macOS (Apple Silicon)** | ✅ Fully Supported | M1/M2/M3/M4 with Metal GPU acceleration |
| **macOS (Intel)** | ⚠️ Limited | May work but not officially tested |
| **Windows 10/11** | ✅ Supported | CPU-based processing; speaker identification not yet available |
| **Linux** | ❌ Not Available | Not planned for beta |

---

## System Requirements

### macOS (Apple Silicon)
| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| **macOS** | 10.15 (Catalina) | 13.0+ (Ventura or newer) |
| **Chip** | Apple M1 | Apple M1 or newer |
| **RAM** | 8 GB | 16 GB |
| **Storage** | 3 GB free | 5 GB free |
| **Internet** | Required for initial setup only | — |

### Windows
| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| **Windows** | Windows 10 (64-bit) | Windows 11 |
| **RAM** | 4 GB | 8 GB |
| **Storage** | 3 GB free | 5 GB free |
| **Internet** | Required for initial setup only | — |

> **macOS Apple Silicon** is the primary platform and benefits from Metal GPU acceleration for significantly faster transcription and summarization. Windows uses CPU-based processing, so expect longer processing times.

### Processing Performance

**macOS (Apple Silicon), default settings:**

| Interview Length | Processing Time |
|------------------|-----------------|
| 6–7 minutes | ~5–10 minutes |
| 15 minutes | ~15–18 minutes |
| 30 minutes | ~25–35 minutes |

Processing happens in the background — you can keep using your computer while it runs.

---

## Download

### Latest Release (v0.2.0)

| Platform | Download |
|----------|----------|
| **macOS (Apple Silicon)** | [Download .dmg]([https://github.com/SourceBuddy-ai/HireScribe-downloads/releases/latest](https://github.com/SourceBuddy-ai/HireScribe-downloads/releases)) |
| **Windows 10/11** | [Download .exe installer]([https://github.com/SourceBuddy-ai/HireScribe-downloads/releases/latest](https://github.com/SourceBuddy-ai/HireScribe-downloads/releases)) |

### macOS Installation
1. Download the `.dmg` file
2. Open the DMG and drag HireScribe to your Applications folder
3. Launch HireScribe and complete the setup wizard (~5 minutes)
4. Start recording or upload your first interview

*Note: On first launch, macOS may show a security prompt. Right-click the app and select "Open" to proceed.*

### Windows Installation
1. Download `HireScribe-Setup-x.x.x.exe`
2. Run the installer and follow the prompts
3. Launch HireScribe and complete the setup wizard (~5 minutes)
4. Start recording or upload your first interview

*Note: Windows may show a SmartScreen prompt on first launch. Click "More info" then "Run anyway" to proceed.*

---

## How It Works

### First-Time Setup

The setup wizard walks you through everything in about 5 minutes:

1. **Hardware detection** — automatically detects your platform and selects the right transcription engine (MLX on Apple Silicon, Faster-Whisper on Intel/Windows)
2. **Disk space check** — confirms you have at least 3 GB free
3. **AI engine setup** — starts the bundled local LLM server (no external service required)
4. **Transcription quality** — choose your preferred Whisper model:
   - **Fast** (`base`, ~150 MB) — quick processing, best for short screenings
   - **Balanced** (`small`, ~500 MB) — recommended for most interviews
   - **Best** (`medium`, ~1.5 GB) — maximum accuracy for senior/executive interviews
5. **Model downloads** — one-time download of your chosen Whisper model and the Qwen3 summarization model

### Daily Use

1. **Record** an interview or **upload** an existing audio file
2. **Wait** for automatic transcription and summarization (runs in the background)
3. **Review** the transcript and AI-generated summaries in the Library
4. **Edit** summaries to add your notes
5. **Export** to Markdown for your records

---

## What's Included

- **MLX Whisper** — GPU-accelerated transcription optimized for Apple Silicon
- **Faster-Whisper** — CPU-based transcription for Intel Macs and Windows
- **llama.cpp** — bundled local LLM server; no external service required
- **Qwen3 (GGUF)** — summarization model optimized for interview analysis; two sizes available:
  - **Qwen3 4B** (~2.5 GB, default) — recommended, requires 8 GB RAM
  - **Qwen3 1.7B** (~1.2 GB) — lighter option for 4 GB RAM machines
- **Speaker diarization** via pyannote.audio — identifies who spoke when (macOS only, optional, adds ~1–2 min)

---

## Beta Program

HireScribe is currently in beta. We're looking for feedback from recruiters who:

- Use macOS with Apple Silicon (M1/M2/M3/M4) or Windows 10/11
- Record or transcribe interviews regularly
- Care about candidate data privacy

### Providing Feedback
- **In-app**: Use the feedback button (bottom-right corner of the app window) to report issues directly


---

## FAQ

**Q: Do I need an internet connection?**
Only for the initial setup to download AI models. After that, HireScribe works completely offline.

**Q: Where is my data stored?**
On macOS, data is stored in `~/Library/Application Support/Hire Scribe/`. On Windows, in `%APPDATA%\Hire Scribe\`. Audio files, transcripts, and summaries never leave your device.

**Q: How accurate is the transcription?**
Whisper-based transcription achieves high accuracy for clear audio. Best results come from a good microphone and minimal background noise. Choose the `medium` model for the highest accuracy.

**Q: Which Whisper model should I choose?**
`small` is the default and the best balance of speed and accuracy for most interviews. Use `medium` for the highest accuracy, or `base` if you need faster processing on a less powerful machine.

**Q: What summary formats does HireScribe generate?**
Every recording automatically gets three formats: **Bullets** (6–8 key takeaways), **Short** (3–4 sentence executive summary), and **Medium** (detailed, organized by topic). All three are editable.

**Q: Can I customize the summary structure?**
Yes. HireScribe ships with 11 built-in templates covering common interview and meeting types. You can also create fully custom templates with your own sections.

**Q: Can I use this for video call recordings?**
Yes. Record audio from your microphone during calls, or upload audio exported from any video conferencing platform.

**Q: Is speaker identification available on Windows?**
Not yet. Speaker diarization is currently macOS only. It will be added to Windows in a future release.

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Cmd/Ctrl + Shift + F` | Open feedback modal |
| `Cmd/Ctrl + ,` | Open Settings |
| `Esc` | Close modals |

---

## Support

- **In-app Help**: See the Help tab within the app
- **Issues**: [GitHub Issues](https://github.com/SourceBuddy-ai/HireScribe-downloads/issues)
- **Email**: tyler@talmarkdigital.com 

---

## License

HireScribe is proprietary software. See [EULA](link) and [Privacy Policy](link) for details.

---

**Stop taking notes. Start having conversations.**
