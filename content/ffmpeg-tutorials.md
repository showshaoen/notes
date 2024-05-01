# Installing ffmpeg on Windows
1. Download [ffmpeg](https://ffmpeg.org/download.html)
2. Unzip the downloaded file and rename the extracted folder to `ffmpeg` and move it into the root of C drive.
3. Run command prompt as administrator and set the envrionment path variable for ffmpeg using the following command.
	```bash
	setx /m PATH "C:\ffmpeg\bin;%PATH%"
	```
4. Restart computer and verify the installation by running:
	```bash
	ffmpeg -version
	```

# ffmpeg Snippets
- https://gist.github.com/liangfu/97f877e311210fa0ae18a31fdd92982e

# Merging Video and Audio
```bash
ffmpeg -i input.mp4 -i input.wav -c:v copy -c:a aac -map 0:v -map 1:a output.mp4
```

| Args     | Description                      |
| -------- | -------------------------------- |
| -c:a aac | audio AAC codec                  |
| -map 0:v | map first input source to video  |
| -map 1:a | map second input source to audio |
Example:
```bash
ffmpeg -i ive.mp4 -i ive.m4a -c:v copy -c:a aac -map 0:v -map 1:a ive-output.mp4
```

# Convert m3u8 stream to mp4
```bash
ffmpeg -i "http://host/folder/file.m3u8" -c copy file.mp4
```

m3u8 to subtitles
```bash
ffmpeg -i "http://host/folder/subs.m3u8" subs.srt
```