### Sample videos
Trimmed to 60s and reduced to 720 for better use as sample videos in website demos.
- [60s-720p](./60s-720p)

### Tools used
Used [ffmpeg](https://ffmpeg.org/download.html) to trim to 60s:
```
ffmpeg -y -ss 30 -i "BigBuckBunny.mp4" -t 60 -c copy "60s/BigBuckBunny.mp4"
```
And to convert quality to 720p if needed:
```
ffmpeg -i "BigBuckBunny.mp4" -vf "scale=-1:720" -c:v libx264 -crf 23 -preset fast -c:a copy "720p/BigBuckBunny.mp4"
```
Note: 23 is the ICQ (quality of compression). 18-28 is a normal range, being 18 a great quality preset and 28 a poor quality one.
### Other
More NASA videos: [https://archive.org/search?query=creator%3A%22NASA%22&and%5B%5D=mediatype%3A%22movies%22](https://archive.org/search?query=creator%3A%22NASA%22&and%5B%5D=mediatype%3A%22movies%22)
### Important note
GitHub Pages is not meant for this. It's speed is bad. If care about speed create an AWS Account. Use S3, create a new general public bucket. Put your files there. As long as you don't exceed 5GB the first year will be free.
