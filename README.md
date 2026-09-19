# 🎬 Automated Reel Generator

A Python-based automation tool that converts user-uploaded images and text descriptions into ready-to-share vertical video reels.

The application continuously monitors a user upload folder, generates **text-to-speech audio** from the description, combines the uploaded images with the generated audio using **FFmpeg**, and creates a **1080×1920 MP4 reel** automatically.

## 🚀 Features

* 📁 Automatically monitors new upload folders
* 📝 Reads descriptions from `desc.txt`
* 🔊 Converts text into speech
* 🖼️ Combines images into a video slideshow
* 🎵 Adds generated audio to the video
* 📱 Creates vertical **9:16 reels (1080×1920)**
* ⚡ Processes folders automatically in the background
* ✅ Tracks completed folders using `done.txt`
* 🎞️ Uses FFmpeg for efficient video processing

## 🛠️ Technologies & Skills

* **Python**
* **File & Folder Automation**
* **Text-to-Speech (TTS)**
* **FFmpeg**
* **Subprocess Management**
* **OS/File System Handling**
* **Video Processing**
* **Automation & Task Queues**
* **MP4 Video Generation**

## 📂 Project Structure

```text
project/
│
├── user_uploads/
│   └── folder_name/
│       ├── desc.txt
│       ├── input.txt
│       └── images/
│
├── static/
│   └── reels/
│       └── generated_reel.mp4
│
├── text_to_audio.py
├── main.py
└── done.txt
```

## ⚙️ How It Works

```text
User Upload
     ↓
New Folder Detected
     ↓
Read desc.txt
     ↓
Text → Speech
     ↓
Generate audio.mp3
     ↓
Combine Images + Audio
     ↓
FFmpeg Video Processing
     ↓
1080 × 1920 MP4 Reel
     ↓
Save to static/reels/
```

## ▶️ How to Run

### 1. Install Python

Make sure Python is installed on your system.

### 2. Install FFmpeg

FFmpeg must be installed and available in your system PATH.

### 3. Prepare an Upload Folder

Create a folder inside:

```text
user_uploads/
```

The folder should contain the required description and input files.

Example:

```text
user_uploads/my_reel/
├── desc.txt
├── input.txt
└── images/
```

### 4. Run the Automation

```bash
python main.py
```

The program continuously checks for new folders and processes them automatically.

## 📌 Output

Generated reels are saved inside:

```text
static/reels/
```

Example:

```text
static/reels/my_reel.mp4
```

## 💡 Key Learning

This project demonstrates how Python can be used to build an **automated content-generation pipeline**, connecting text processing, text-to-speech, file-system automation, and video processing into a single workflow.

## 👩‍💻 Skills Demonstrated

**Python | Automation | Text-to-Speech | FFmpeg | Video Processing | File Handling | Subprocess | Content Generation**
