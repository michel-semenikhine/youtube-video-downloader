# YouTube Video Downloader - SEMENIKHINE MICHEL

This program allows you to download YouTube videos in mp4 in the desired resolution.
It lists available video and audio formats and provides an easy way to download and combine them into a single MP4 file.

## Features
- Lists available video and audio formats for a YouTube URL.
- Allows you to select specific video and audio formats by ID.
- Downloads the selected video and audio separately and merges them into a single MP4 file.
- Converts the downloaded content into a compatible format using FFmpeg for easy playback.

## Requirements
- Download and Install FFMPEG via the [official website](https://www.ffmpeg.org)

## How to Use
1. **Run the Program**: You can download the latest build of the program from the [Releases](https://github.com/michel-semenikhine/youtube-video-downloader/releases) section.
\
Simply launch the program.

2. **Enter the YouTube URL**: When prompted, paste the URL of the YouTube video you want to download.

3. **Choose Video and Audio Formats**:
   - The program will display a list of available formats (video and audio). 
   - Each format will be listed with its ID, resolution, file size (if known) and framerate.
   - Enter the **Video ID** and **Audio ID** you want to download.

4. **Download and Merge**: The program will download the video and audio files separately and automatically merge them into a single MP4 file.

5. **Finish**: Once the download and merging are complete, the program will notify you that the process is finished.

## Example
Downloading a video in 1080p :
```bash
Enter YouTube URL : https://www.youtube.com/watch?v=dQw4w9WgXcQ

List of available formats :

ID : 233  | Resolution : audio only | Size : Unknown  | FPS :  N/A  | Format : mp4 
ID : 234  | Resolution : audio only | Size : Unknown  | FPS :  N/A  | Format : mp4 
ID : 597  | Resolution :  256x144   | Size :  848491  | FPS :   13  | Format : mp4 
ID : 160  | Resolution :  256x144   | Size : 1864273  | FPS :   25  | Format : mp4 
ID : 394  | Resolution :  256x144   | Size : 1473724  | FPS :   25  | Format : mp4 
ID : 133  | Resolution :  426x240   | Size : 3020923  | FPS :   25  | Format : mp4 
ID : 395  | Resolution :  426x240   | Size : 2900181  | FPS :   25  | Format : mp4 
ID : 134  | Resolution :  640x360   | Size : 5680516  | FPS :   25  | Format : mp4 
ID :  18  | Resolution :  640x360   | Size :   None   | FPS :   25  | Format : mp4 
ID : 396  | Resolution :  640x360   | Size : 5083621  | FPS :   25  | Format : mp4 
ID : 135  | Resolution :  854x480   | Size : 8685524  | FPS :   25  | Format : mp4 
ID : 397  | Resolution :  854x480   | Size : 8577091  | FPS :   25  | Format : mp4 
ID : 136  | Resolution :  1280x720  | Size : 16782510 | FPS :   25  | Format : mp4 
ID : 398  | Resolution :  1280x720  | Size : 15710398 | FPS :   25  | Format : mp4 
ID : 137  | Resolution : 1920x1080  | Size : 80170781 | FPS :   25  | Format : mp4 
ID : 399  | Resolution : 1920x1080  | Size : 29010461 | FPS :   25  | Format : mp4 

Enter VIDEO ID to download : 137

Enter AUDIO ID to download : 233

Downloading...
[youtube] Extracting URL: https://www.youtube.com/watch?v=dQw4w9WgXcQ 
[youtube] dQw4w9WgXcQ: Downloading webpage 
[youtube] dQw4w9WgXcQ: Downloading ios player API JSON 
[youtube] dQw4w9WgXcQ: Downloading mweb player API JSON 
[youtube] dQw4w9WgXcQ: Downloading m3u8 information 
[info] dQw4w9WgXcQ: Downloading 1 format(s): 137+233 
[download] Destination: Rick Astley - Never Gonna Give You Up (Official Music Video).f137.mp4 
[download] 100% of   76.46MiB in 00:00:01 at 55.48MiB/s
[hlsnative] Downloading m3u8 manifest 
[hlsnative] Total fragments: 39 
[download] Destination: Rick Astley - Never Gonna Give You Up (Official Music Video).f233.mp4 
[download] 100% of    1.25MiB in 00:00:00 at 1.64MiB/s
[Merger] Merging formats into "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4" 
Deleting original file Rick Astley - Never Gonna Give You Up (Official Music Video).f137.mp4 (pass -k to keep) 
Deleting original file Rick Astley - Never Gonna Give You Up (Official Music Video).f233.mp4 (pass -k to keep) 
[VideoConvertor] Not converting media file "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"; already is in target format mp4 
Downloading finished !
```

The video will be located in the same folder where you launched the program.

# Note
This youtube video downloader doesn't bypass YouTube’s restrictions such as age restrictions or private online posting. Only videos that can be viewed without a YouTube account can be downloaded.
