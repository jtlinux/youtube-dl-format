# youtube-dl-formats
Search for and download a specific format with youtube-dl

This script displays a YouTube video's available formats and asks the user to choose a format to download.</br>
The user's most recent item on the xclip clipboard is used as input for the video download commands.

**Dependencies:**

 - youtube-dl
 - xclip

**My reasons for uploading this script:**

I'd be happy to receive help. I'm new to scripting. This is a script I wrote and have recently been working on because I personally use it often. I often have to download videos or audio for work or personal use. I have very limited bandwidth, which makes downloading preferable to streaming, and it also makes format selection essential.

**TO-DO:**

 - Replace xclip clipboard with a clipboard that retains more than one entry. (I would like to be able to search the clipboard for the most recent YouTube URL.)
 - Have youtube-dl download video information only once. (It currently downloads twice: once with `youtube-dl -F` command and again with `youtube-dl -f` command).
 - Supress messages from youtube-dl about the download of video information, while retaining format information from `-F`.
