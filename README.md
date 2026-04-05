# yt-dlp accessory script
this script basically abstracts away two commands to download youtube videos, so all i have to do is enter a url, and accept or reject to get it kicked off

- it will pull all available video and audio formats, and preselect the best most compatible audio and video files
- then it will ask download? yes / no
- hit yes to continue
- it will require yt-dlp to be updated to the latest version

### formats available
yt-dlp -F "https://www.youtube.com/watch?v=-In1EPx9t8M"

### dl highest quality audio video
yt-dlp --continue --retries 10 --fragment-retries 10 --merge-output-format mp4 --no-check-certificate -f "234+270" -P "$HOME/Downloads" "https://www.youtube.com/watch?v=-In1EPx9t8M"