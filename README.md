# 🎬 Automated Reel Generator

A Python-based automated reel generation system that converts uploaded images and text descriptions into vertical video reels with generated voice narration.

The project monitors user-uploaded content, converts text into audio, processes images using **FFmpeg**, and generates a final MP4 reel automatically.

## 🚀 Features

* 📁 Detects newly uploaded folders
* 📝 Reads text descriptions from uploaded content
* 🔊 Converts text into speech using Python
* 🖼️ Processes images into a video sequence
* 🎵 Combines generated audio with video
* 📱 Generates vertical **1080 × 1920** reels
* ⚙️ Uses FFmpeg for video processing
* ✅ Tracks processed folders using `done.txt`
* 🔄 Automatically checks for new content

## 🛠️ Technologies & Skills

**Programming & Automation**

* Python
* File & Folder Handling
* Process Automation
* Subprocess Management

**AI / Audio**

* Text-to-Speech (TTS)
* Automated Voice Generation

**Video Processing**

* FFmpeg
* Image-to-Video Processing
* Audio-Video Synchronization
* MP4 Generation
* Vertical Video / 9:16 Format

## 📂 Project Structure

```text
Automated-Reel-Generator/
│
├── 📁 sample_images/          # Sample images for testing
├── 📁 static/                 # Generated/static application files
├── 📁 templates/              # Application templates
├── 📁 user_uploads/           # User-uploaded content
│
├── 📄 config.py               # Project configuration
├── 📄 done.txt                # Tracks processed folders
├── 📄 ffmpeg_command.txt      # FFmpeg command/reference
├── 📄 generate_process.py     # Reel generation process
├── 📄 main.py                 # Main application
├── 📄 reel.mp4                # Sample generated reel
├── 📄 sample_input_ffmpeg.txt # Sample FFmpeg input
├── 📦 template.zip            # Project/template archive
└── 📄 text_to_audio.py        # Text-to-speech functionality
```

## 🔄 Workflow

```text
User Upload
     ↓
Folder Detection
     ↓
Read Description
     ↓
Text-to-Speech
     ↓
Generate Audio
     ↓
Process Images
     ↓
FFmpeg Video Generation
     ↓
Combine Video + Audio
     ↓
Generate Final Reel
```

## ▶️ How It Works

1. A new folder is placed inside `user_uploads/`.
2. The system identifies folders that have not been processed.
3. The description text is read from the uploaded content.
4. `text_to_audio.py` generates the corresponding audio.
5. FFmpeg processes the images and audio into a video.
6. The final reel is generated in MP4 format.
7. The folder name is added to `done.txt` to prevent duplicate processing.

## 🎞️ Output

The project generates a vertical social-media-ready reel in:

**1080 × 1920 resolution — 9:16 aspect ratio**

A sample output is included as:

```text
reel.mp4
```

## 💡 Key Learning

This project demonstrates how Python can automate a complete **content-to-video generation pipeline**, combining text processing, text-to-speech, file-system automation, and FFmpeg-based video processing.

## 👩‍💻 Skills Demonstrated

**Python | Automation | Text-to-Speech | FFmpeg | Video Processing | File Handling | Subprocess | Audio Processing | Content Generation**
