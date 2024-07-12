# Playlist Downloader and Merger

This project provides a Python script to download all videos from a YouTube playlist and merge them into a single video file while maintaining the order of the clips.

## Features

### Parallel Downloads
- **Efficiency**: Downloads videos in parallel to speed up the process.
- **Customization**: Option to set the number of concurrent downloads.

### Efficient Merging
- **Order Preservation**: Maintains the order of videos as they appear in the playlist.
- **Fast and Reliable**: Utilizes `ffmpeg` for fast and efficient video merging.

### Clean Up
- **Space Management**: Deletes individual video files after merging to free up disk space.
- **Optional**: Can be configured to keep the individual files if needed.

## Scope

This project is designed to be a comprehensive solution for downloading and merging videos from a YouTube playlist. It's suitable for users who need to:

- Archive a playlist for offline viewing.
- Create a continuous video from multiple parts.
- Consolidate educational content for easier consumption.

## Use Cases

### Educational Content
- **Students**: Download and merge lecture series or tutorial playlists to create a single, uninterrupted video for easy studying.
- **Teachers**: Compile lesson videos into one file for seamless presentation.

### Entertainment
- **Movie Buffs**: Combine episodes of a web series or a list of related videos into a single file for uninterrupted viewing.
- **Content Creators**: Download and merge clips for video editing and production.

### Professional Use
- **Researchers**: Archive conference talks, presentations, or webinars.
- **Corporate Training**: Merge training modules from various sources into one comprehensive training video.

## Installation

1. **Clone the Repository**:

    ```sh
    git clone https://github.com/yourusername/playlist-downloader-merger.git
    cd playlist-downloader-merger
    ```

2. **Install Required Libraries**:

    ```sh
    pip install yt-dlp moviepy ffmpeg-python
    ```

3. **Install FFmpeg**:
   
   - **Windows**: Download from [ffmpeg.org](https://ffmpeg.org/download.html) and add to your PATH.
   - **macOS**: Install via Homebrew:
   
     ```sh
     brew install ffmpeg
     ```
   
   - **Linux**: Install via package manager, e.g., for Ubuntu:
   
     ```sh
     sudo apt update
     sudo apt install ffmpeg
     ```

## Usage

1. **Run the Script**:

    ```sh
    python download_playlist.py
    ```

2. **Input Playlist URL and Download Path**:

    - Enter the URL of the YouTube playlist when prompted.
    - Enter the download path (leave empty for the current directory).

The script will download all videos in the playlist, merge them into a single video file named `merged_video.mp4` in the specified download path, and then delete the individual video files.

## Example

```sh
python download_playlist.py
