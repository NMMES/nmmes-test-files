# NMMES-test-files
The respository contains a number of files used in testing of NMMES's operational status.

### Naming Scheme
```
file_name-(usage)-resolution[attribute1][attribute2]-resolution[attribute1][attribute2]-missing.format
```

- **file name** should be located at the begining of the file and be seperated by underscores(_).
- **usage** should represent the reason it is being included in this repo, such as what test it is used for.
- **resolution** should be listed for at least one stream of each type
    - Video: The vertical resolution of the video (1080p for a 1420x1080 video)
    - Audio: The number of audio channels in the stream (6ch for 5.1 audio)
    - Subtitle: The format of the subtitle stream (pgs, vob, srt, ass)
    - **attributes** can list as many properties as you like, but try to keep it concise
- **missing** displays that the file does not have a specific stream (possibilities are novid/noaud/nosub)

##### Examples
```
hale_bopp_1-(invalidCrop240p)-480p[yuv420p][mpeg1]-noadu-nosub.mpg
sintel_trailer-(base)-480p[yuv420p][x264]-2ch[aac]-nosub.mp4
hancock_trailer-(upconvert)-480p[yuv420p][x264]-2ch[aac]-pgs.mp4
```
