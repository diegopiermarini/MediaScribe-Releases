# MediaScribe

**Turn audio and video into text and subtitles, right on your PC.**
Drop in a recording (a meeting, an interview, a lecture, a video) and MediaScribe gives you back the text, the subtitles and, if you like, a translation into other languages. It also recognises who is speaking.

It runs on Windows, with no account and no subscription. Your files are never uploaded anywhere: all the work happens on your computer.

👉 **[Download the latest version](https://github.com/diegopiermarini/MediaScribe-Releases/releases/latest)**: on the page that opens, under **Assets**, click `MediaScribe-Setup-<version>.exe`.

---

## What you can do

- **Transcribe** audio and video files, several at once or a whole folder.
- **Record** a meeting or a call straight from the app: your voice and what the PC plays (Teams, Zoom, Meet, videos). Press Stop and the transcription starts on its own.
- **Get subtitles** (`.srt`, plus `.vtt` from the settings), already split into readable, well-timed lines.
- **Get the text** (`.txt`) in paragraphs, with the time at the start of each paragraph if you want it, and a **Word document** (`.docx`).
- **Know who is speaking**: in recordings with several voices the text marks "Speaker 1", "Speaker 2"… automatically. At the end you can type their real names ("Mark", "Julia") and the app puts them in every file.
- **Translate** the result into one or more languages (42 available), also on your PC; even later, from the results screen.
- **Get a summary**: from the results screen, "Summary" writes a short summary of the recording (in short, main points, decisions, things to do), on your PC.
- **Pick up where you left off**: the start screen lists your **Recent** transcriptions. **Open** brings back their results, even after closing the app, to rename people, make the summary or translate again.
- **Help the recognition** of names and special terms by typing them in "Words to recognise".
- **Never lose your work**: during long transcriptions the PC doesn't go to sleep and the part already done is saved every minute. If the job is interrupted, next time it picks up where it left off.

Files you can open: MP3, WAV, M4A, FLAC, AAC, OGG, OPUS, WMA, MP4, MKV, AVI, MOV, WEBM, M4V.
The interface is available in English and Italian, with a light or dark theme.

---

## Requirements

| | Minimum | Recommended |
|---|---|---|
| System | Windows 10 or 11, 64-bit | Windows 11 |
| Memory (RAM) | 4 GB | 8 GB or more (needed for the most accurate models) |
| Disk space | about 1 GB | 3-5 GB if you want several models and translation |
| Internet | only the first time, to download the models | |
| Graphics card | not needed | NVIDIA GTX 10 series or newer with at least 4 GB: transcription becomes many times faster |

If you have a suitable NVIDIA card, MediaScribe notices and uses it on its own: there is nothing to install.

---

## Installation

1. **[Download](https://github.com/diegopiermarini/MediaScribe-Releases/releases/latest)** `MediaScribe-Setup-<version>.exe`.
2. Open it and follow the steps. No administrator rights are needed: the app is installed for your user only.
3. When it's done, you'll find MediaScribe in the Start menu.

**Windows says "Windows protected your PC"?** That's normal for programs that aren't widely known yet. Click **More info**, then **Run anyway**. If you want to be sure the file is exactly the one published here, see [Check the downloaded file](#check-the-downloaded-file).

---

## How to use it

1. **Drag** one or more files into the window (or click **Choose files**).
2. Choose **what you need**: subtitles, text or both.
3. If you like, pick languages under **Also translate to**.
4. Click **Transcribe**. You'll see the progress, the time left and the last sentence understood.
5. When it's done, your files are in the folder you chose, with the **Open**, **Copy text** and **Show in folder** buttons.
6. Later, find the job again under **Recent** on the start screen.

**Which model should I pick?** The model is the "brain" that listens to the audio: bigger ones are more accurate but slower. The app shows you the one **recommended for your PC**. In short:

| Model | Download | When to use it |
|---|---|---|
| Tiny, Base | 75-145 MB | less powerful PCs, quick tries |
| Small | 485 MB | a good balance on almost any PC |
| Medium | 1.5 GB | more accuracy, PCs with 8 GB of memory |
| Turbo | 1.6 GB | as accurate as Medium and faster: great for meetings |
| Large | 3.1 GB | the highest accuracy, NVIDIA card only |

Each model is downloaded only once, the first time you use it. The same goes for the translator (about 500 MB), speaker recognition (about 34 MB) and summaries (about 3 GB).

---

## Recording

Click **Record** on the start screen, choose your voice (microphone), the PC's audio (calls, videos) or both, and start. The recording is saved as it goes; **Stop and transcribe** turns it into text right away. When you record both, the transcript calls you **You** (or by your name, if you type it on the recording screen) and tells the other people apart. Tick **Make a summary at the end too** to get the summary right after the transcript. Please tell people when you record them, and use headphones: with speakers the microphone picks up the others a second time.

---

## Privacy

- Your audio, video and texts **stay on your PC**: transcription, translation, speaker recognition and summaries all run on your computer.
- MediaScribe only uses the internet to:
  - download the models the first time (from Hugging Face) and, if you have an NVIDIA card, the library needed to use it (NVIDIA's official package);
  - check whether a new version is available (from this page).
- In the settings you can choose **Google Translate** instead of translating on your PC, if you want: in that case the text to translate is sent to Google. It's off by default.

---

## Updates

When a new version comes out, MediaScribe tells you with a notice at the top. Click **Update now**: the app downloads the new version, checks that it's intact, updates itself and reopens. Your settings and the models already downloaded are kept.

---

## Uninstalling

From **Windows Settings → Apps → MediaScribe → Uninstall**.
While uninstalling you can choose whether to keep your settings and the downloaded models (handy if you plan to reinstall). Your audio and video files and the texts you created are never deleted.

---

## Check the downloaded file

Next to the installer, every version has a `SHA256SUMS.txt` file with the installer's "fingerprint". To check that the file you downloaded is identical to the one published:

1. Open **PowerShell** in the folder where you downloaded the installer.
2. Type: `Get-FileHash .\MediaScribe-Setup-<version>.exe`
3. The value shown must match the one in `SHA256SUMS.txt` (upper or lower case doesn't matter).

Automatic updates do this check on their own.

---

## Frequently asked questions

**It's slow.** Pick a smaller model, or the one recommended for your PC. With a suitable NVIDIA card, transcription is much faster.

**Speaker recognition got it wrong.** It works well when voices are different and people speak one at a time; with very similar voices, background noise or people talking over each other it can get confused. With a single voice it writes no names.

**I closed the app halfway through a long file.** Open it again and transcribe the same file with the same model: it picks up where it left off. The part already done is saved anyway as `<name>_partial`.

**How good are the summaries?** They are made by a small AI model on your PC: good at the main points, but they can get a detail wrong. Check important details in the transcript; the summary file reminds you.

**Where are my files?** Next to the original files, or in the folder you chose under "Save to". From the final screen, **Show in folder** opens it.

---

## Built with

MediaScribe is built on open-source components, including: [faster-whisper](https://github.com/SYSTRAN/faster-whisper) and the [Whisper](https://github.com/openai/whisper) models (MIT) for transcription, [M2M100](https://huggingface.co/facebook/m2m100_418M) (MIT) for translation, [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) (Apache-2.0) with the pyannote (MIT) and 3D-Speaker (Apache-2.0) models for speaker recognition, [Llama 3.2](https://www.llama.com/llama3_2/license/) 3B Instruct (Llama 3.2 Community License) for summaries, [FFmpeg](https://ffmpeg.org) (GPL) to read video files, and [Qt for Python](https://www.qt.io/qt-for-python) (LGPL) for the interface.

**Built with Llama.** Llama 3.2 is licensed under the Llama 3.2 Community License, Copyright © Meta Platforms, Inc. All Rights Reserved.
