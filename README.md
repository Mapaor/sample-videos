### Sample videos
Trimmed to 60s and reduced to 720 for better use as sample videos in website demos
### TIPs
Use [ffmpeg](https://ffmpeg.org/download.html) to trim to 60s:
```
ffmpeg -y -ss 30 -i "BigBuckBunny.mp4" -t 60 -c copy "60s/BigBuckBunny.mp4"
```
Or to convert quality to 720p if needed:
```
ffmpeg -i "BigBuckBunny.mp4" -vf "scale=-1:720" -c:v libx264 -crf 23 -preset fast -c:a copy "720p/BigBuckBunny.mp4"
```
Note: 23 is the ICQ (quality of compression). 18-28 is a normal range, being 18 a great quality preset and 28 a poor quality one.
### Other
More NASA videos: [https://archive.org/search?query=creator%3A%22NASA%22&and%5B%5D=mediatype%3A%22movies%22](https://archive.org/search?query=creator%3A%22NASA%22&and%5B%5D=mediatype%3A%22movies%22)
