# youtube-dl-formats
Search for and download a specific format with youtube-dl

This script displays a YouTube video's available formats and asks the user to choose a format to download.<br>
The user's most recent item on the xclip clipboard is used as input for the video download commands.<br>
Alternatively, add a format to the command to download it (e.g. `youtube-dl-formats 43` will work as `youtube-dl -f 43`).

**Dependencies:**

 - youtube-dl
 - xclip
 - vlc
 - paplay
 - notify-send (libnotify-bin)

**My reasons for uploading this script:**

I'd be happy to receive help. I'm new to scripting. This is a script I wrote and have recently been working on because I personally use it often. I often have to download videos or audio for work or personal use. I have very limited bandwidth, which makes downloading preferable to streaming, and it also makes format selection essential.

**TO-CODE/WISH LIST:**

 - [HIGH priority] Check that a YouTube video URL exists on the clipboard before attempting to fetch format information. Return an error and exit if URL does not exist in clipboard.
 - [LOW] Replace xclip clipboard with a clipboard that retains more than one entry. (I would like to be able to search the clipboard for the most recent YouTube URL.)
 - [LOW] Have youtube-dl download video information only once. (It currently downloads twice: once with `youtube-dl -F` command and again with `youtube-dl -f` command).
 - [LOW] Supress messages from youtube-dl about the download of video information, while still showing the format information from `-F`.
