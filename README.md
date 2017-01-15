S-ul uploader for linux
=====================

Originally written by Sunmock Yang as a puush uploader. 

Ported for s-ul by Liam Svanåsbakken Crouch. Additionally, support for screenfetch was added.

Please note this README is from the original puush uploader, but all existing features are left untouched.

Takes screenshots and uploads them to s-ul using the s-ul API and copies the link to clipboard. Recommended for set up with keyboard shortcuts
<br>Utilises __gnome-screenshot__ for taking screenshots, __zenity__ for file uploads (both included in Ubuntu).

## Instructions
- Clone or download the repo
- In file "s-ul" add your s-ul API key to SUL_API_KEY
  - (You can find your API key at [https://s-ul.eu/settings.php](https://s-ul.eu/settings.php) )
- Make it executable using __chmod +x s-ul__
- Place this file wherever you want (recommended: /usr/local/bin)
- Set up keyboard shortcuts within linux
  - (in Ubuntu it's system settings > keyboard > keyboard shortcuts > custom shortcuts)
  - Log out for the changes to take place
  - Here's what it looks like for mine: ![S-Ul keyboard setup](http://puu.sh/cOyVz/8dcb1cd498.png)

### Commands
``` bash
s-ul -a		# capture desktop
s-ul -b		# area capture
s-ul -c		# capture window
s-ul -d		# file upload
s-ul -f     # run screenfetch and capture desktop

s-ul -h  	  # help
```

## Dependencies
 - gnome-screenshot
 - curl
 - zenity
 - xclip
 - notify-send
 - screenfetch
 - jq

