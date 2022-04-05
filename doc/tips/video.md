# Video

## How to get technical information about a video

```bash
mediainfo myfile.avi
```

## How to rotate a video to 90 degrees.

```bash
ffmpeg -i input -vcodec libx264 -preset medium -crf 24 -threads 0 -vf transpose=1 -acodec copy output.mkv
```

[Back to index](../README.md)
