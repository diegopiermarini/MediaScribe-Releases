# MediaScribe

**Turn audio and video into text and subtitles, right on your PC.**
Drop in a recording (a meeting, an interview, a lecture, a video) and MediaScribe gives you back the text, the subtitles and, if you like, a translation into other languages. It also recognises who is speaking.

It runs on Windows, with no account and no subscription. Your files are never uploaded anywhere: all the work happens on your computer.

👉 **[Download the latest version](https://github.com/diegopiermarini/MediaScribe-Releases/releases/latest)**: on the page that opens, under **Assets**, click `MediaScribe-Setup-<version>.exe`.

---

## What's new in 0.22.0

- **Correct the transcript**: the new **Correct** button on the results screen shows every phrase with its time and who says it. Fix a word, change who is speaking, join two phrases or split one in two, and **listen to a phrase** to check a word you're not sure about. **Find and replace** fixes a misspelt name everywhere at once. When you save, every file is updated: text, subtitles (timing included), Word, PDF and Markdown. It works on transcriptions made with this version or later.

---

## What you can do

- **Transcribe** audio and video files, several at once or a whole folder.
- **Record** a meeting or a call straight from the app: your voice and what the PC plays (Teams, Zoom, Meet, videos), with the **text appearing live**. Press Stop and the full transcription starts on its own. When you are in a call, MediaScribe offers to record it.
- **Get subtitles** (`.srt`, plus `.vtt` from the settings), already split into readable, well-timed lines.
- **Get the text** (`.txt`) in paragraphs, with the time at the start of each paragraph if you want it, a **Word document** (`.docx`), a **PDF** or **Markdown**.
- **Correct the result**: fix words, change who is speaking, join or split phrases and listen to each one; saving updates every file.
- **Know who is speaking**: in recordings with several voices the text marks "Speaker 1", "Speaker 2"… automatically. At the end you can type their real names ("Mark", "Julia") and the app puts them in every file.
- **Translate** the result into one or more languages (42 available), also on your PC; even later, from the results screen.
- **Get a summary**, on your PC, shaped for the recording: decisions and things to do for a meeting, questions and answers for an interview, key ideas for a lecture. **Copy summary** puts it on the clipboard, ready to paste into an email or a chat; translations include the summary too.
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

Each model is downloaded only once, the first time you use it. The same goes for the translator (about 500 MB) and summaries (about 3 GB). Speaker recognition is already included in the installer. In **Settings → Space used by models** you can see how much each one takes and delete the ones you don't use.

---

## Recording

Click **Record** on the start screen, choose your voice (microphone), the PC's audio (calls, videos) or both, and start. The recording is saved as it goes; **Stop and transcribe** turns it into text right away. When you record both, the transcript calls you **You** (or by your name, if you type it on the recording screen) and tells the other people apart. Tick **Make a summary at the end too** to get the summary right after the transcript. While you record, the **live text** shows what is being said a few seconds later (on PCs without a suitable NVIDIA card it needs a processor with at least 6 threads).

Please tell people when you record them: the recording screen has a ready sentence you can say or paste in the call's chat (**Copy the notice**). Use headphones: with speakers the microphone picks up the others a second time.

If the app is open while you are in a call (Teams, Zoom, Webex, WhatsApp, or a call in the browser), it offers to record it. It only looks at which program is using the microphone, the same thing Windows shows with its microphone icon; nothing is listened to until you press **Record**.

---

## Privacy

*Privacy policy of MediaScribe, the app published on this page and in the Microsoft Store. Last updated: 23 November 2026.*

**In short: MediaScribe collects no personal data.** There is no account, no advertising, no analytics and no tracking. Your recordings, files, transcripts, translations and summaries stay on your PC: they are never sent to us or to anyone else.

**What stays on your PC**

- The audio and video you open or record, and everything MediaScribe makes from them: transcription, speaker recognition, translation and summaries all run on your computer.
- Your settings, the list of recent jobs and the downloaded models, in the `.mediascribe` folder of your Windows user profile.

**When MediaScribe uses the internet**

- To download the models the first time they are needed, from Hugging Face, and, on PCs with a suitable NVIDIA card, NVIDIA's official library from the Python Package Index (PyPI).
- In the version downloaded from this page: to check whether a new version is out and, when you click **Update now**, to download it from GitHub. The Microsoft Store version is updated by the Store.
- Only if you choose **Google Translate** in the settings (it's off by default): the text to translate is sent to Google, under Google's privacy policy.

These requests carry none of your files or texts (except the text sent to Google, if you choose it). Like any download, the services involved see your IP address.

**Microphone and recording**

MediaScribe uses the microphone and the PC's audio only while you record, after you press **Record**. To offer to record a call, it checks which program is using the microphone (the same information Windows shows with its microphone icon); it doesn't listen to anything. Please tell people when you record them.

**Children**

MediaScribe is not aimed at children and collects no data from anyone.

**Removing your data**

Your transcripts are ordinary files: delete them as you like. The uninstaller offers to remove your settings and the downloaded models; **Settings → Space used by models** removes models at any time. Uninstalling the Microsoft Store version doesn't remove the `.mediascribe` folder in your user profile: delete it by hand if you want.

**Contact**

Questions about privacy: mediascribe.app@outlook.com. Any change to this policy will appear in this section, with a new date.

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
