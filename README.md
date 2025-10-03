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
GitHub Pages is not meant for this. It's speed is bad. If you care about speed you should use a bucket for storage in the cloud.

#### With Appwrite
Create an account, create a project, create a bucket, in settings enable file security, start putting files. 5GB free for everyone 150GB for students (it's a lot!).

Examples:


#### With S3
Create an AWS Account, use S3, and create a new general public bucket. Put your files there, as long as you don't exceed 5GB the first year will be free.

Example files (may expire past March 2026): 
- [https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/BigBuckBunny.mp4](https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/BigBuckBunny.mp4)
- [https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/ElephantsDream.mp4](https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/ElephantsDream.mp4)
- [https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/Sintel.mp4](https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/Sintel.mp4)
- [https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/TearsOfSteel.mp4](https://bucket-general-public-marti.s3.eu-west-1.amazonaws.com/60s-720p/gtv-videos-bucket/TearsOfSteel.mp4)
