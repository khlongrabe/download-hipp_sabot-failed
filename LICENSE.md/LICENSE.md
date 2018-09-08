hans@hans-GA-78LMT-USB3:~$ sudo apt-add-repository ppa:nilarimogard/webupd8
[sudo] password for hans: 
 The main Web Upd8 PPA maintained by: http://www.webupd8.org/

To add this PPA, simply paste this in a terminal:
sudo add-apt-repository ppa:nilarimogard/webupd8

Packages in this PPA: audacious, ap-hotspot, awn-applet-radio, awn-applet-wm, calise, cmus, dockbarx, dockbarx-themes-extra, dropbox-share, emerald, exaile, fbmessenger, gnome-subtitles, gnome-window-applets, grsync, grive, gthumb, launchpad-getkeys, mc, mdm (Mint Display Manager), minitunes, minitube, musique, notifyosdconfig, nautilus-columns, powertop, ppa-purge, rosa-media-player, fixed pulseaudio-equalizer, subtitleeditor, syncwall, umplayer, unity-reboot, wimlib, youtube-dl, xfce4-dockbarx-plugin, xournal, yad, yarock and others. Almost all packages are updated to their latest version.

For other (specialized) PPAs we maintain, see: https://launchpad.net/~webupd8team
 More info: https://launchpad.net/~nilarimogard/+archive/ubuntu/webupd8
Press [ENTER] to continue or Ctrl-c to cancel adding it.

Hit:1 http://archive.canonical.com/ubuntu bionic InRelease
Hit:2 http://ppa.launchpad.net/embrosyn/cinnamon/ubuntu bionic InRelease       
Get:3 http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu bionic InRelease [15,4 kB]
Hit:4 http://repository.cliqz.com/dist/debian-release stable InRelease         
Hit:5 ftp://ftp.fu-berlin.de/linux/ubuntu bionic InRelease                     
Hit:6 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-updates InRelease             
Get:7 http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu bionic/main amd64 Packages [10,9 kB]
Hit:8 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-backports InRelease           
Get:9 http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu bionic/main i386 Packages [10,6 kB]
Hit:10 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-security InRelease           
Get:11 http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu bionic/main Translation-en [7.708 B]
Fetched 44,5 kB in 2s (29,4 kB/s)                                    
Reading package lists... Done
hans@hans-GA-78LMT-USB3:~$ sudo apt-get update
Hit:1 http://repository.cliqz.com/dist/debian-release stable InRelease
Hit:2 http://archive.canonical.com/ubuntu bionic InRelease 
Hit:3 http://ppa.launchpad.net/embrosyn/cinnamon/ubuntu bionic InRelease
Hit:4 http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu bionic InRelease    
Hit:5 ftp://ftp.fu-berlin.de/linux/ubuntu bionic InRelease                     
Hit:6 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-updates InRelease
Hit:7 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-backports InRelease
Hit:8 ftp://ftp.fu-berlin.de/linux/ubuntu bionic-security InRelease
Reading package lists... Done
hans@hans-GA-78LMT-USB3:~$ sudo apt-get install youtube-dl
Reading package lists... Done
Building dependency tree       
Reading state information... Done
youtube-dl is already the newest version (2018.03.14-1).
The following package was automatically installed and is no longer required:
  binutils-common:i386
Use 'sudo apt autoremove' to remove it.
0 upgraded, 0 newly installed, 0 to remove and 8 not upgraded.
hans@hans-GA-78LMT-USB3:~$ youtube-dl https://www.youtube.com/watch?v=V38psI8WIvI
[youtube] V38psI8WIvI: Downloading webpage
[youtube] V38psI8WIvI: Downloading video info webpage
[youtube] V38psI8WIvI: Extracting video information
[youtube] V38psI8WIvI: Downloading js player vflvABTsY
ERROR: Signature extraction failed: Traceback (most recent call last):
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1191, in _decrypt_signature
    video_id, player_url, s
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1102, in _extract_signature_function
    res = self._parse_sig_js(code)
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1163, in _parse_sig_js
    jscode, 'Initial JS player signature function name', group='sig')
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/common.py", line 796, in _search_regex
    raise RegexNotFoundError('Unable to extract %s' % _name)
youtube_dl.utils.RegexNotFoundError: Unable to extract Initial JS player signature function name; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
 (caused by RegexNotFoundError('Unable to extract \x1b[0;34mInitial JS player signature function name\x1b[0m; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.',)); please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
hans@hans-GA-78LMT-USB3:~$ youtube-dl --verbose
[debug] System config: []
[debug] User config: []
[debug] Custom config: []
[debug] Command-line args: ['--verbose']
[debug] Encodings: locale UTF-8, fs utf-8, out UTF-8, pref UTF-8
[debug] youtube-dl version 2018.03.14
[debug] Python version 3.6.5 (CPython) - Linux-4.15.0-33-generic-x86_64-with-Ubuntu-18.04-bionic
[debug] exe versions: ffmpeg 3.4.4-0ubuntu0.18.04.1, ffprobe 3.4.4-0ubuntu0.18.04.1, phantomjs 2.1.1, rtmpdump 2.4
[debug] Proxy map: {}
Usage: youtube-dl [OPTIONS] URL [URL...]

youtube-dl: error: You must provide at least one URL.
hans@hans-GA-78LMT-USB3:~$ youtube-dl --verbose https://www.youtube.com/watch?v=V38psI8WIvI^C
hans@hans-GA-78LMT-USB3:~$ youtube-dl --verbose  youtube-dl https://www.youtube.com/watch?v=V38psI8WIvI
[debug] System config: []
[debug] User config: []
[debug] Custom config: []
[debug] Command-line args: ['--verbose', 'youtube-dl', 'https://www.youtube.com/watch?v=V38psI8WIvI']
[debug] Encodings: locale UTF-8, fs utf-8, out UTF-8, pref UTF-8
[debug] youtube-dl version 2018.03.14
[debug] Python version 3.6.5 (CPython) - Linux-4.15.0-33-generic-x86_64-with-Ubuntu-18.04-bionic
[debug] exe versions: ffmpeg 3.4.4-0ubuntu0.18.04.1, ffprobe 3.4.4-0ubuntu0.18.04.1, phantomjs 2.1.1, rtmpdump 2.4
[debug] Proxy map: {}
ERROR: 'youtube-dl' is not a valid URL. Set --default-search "ytsearch" (or run  youtube-dl "ytsearch:youtube-dl" ) to search YouTube
Traceback (most recent call last):
  File "/usr/lib/python3/dist-packages/youtube_dl/YoutubeDL.py", line 785, in extract_info
    ie_result = ie.extract(url)
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/common.py", line 440, in extract
    ie_result = self._real_extract(url)
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/generic.py", line 2112, in _real_extract
    % (url, url), expected=True)
youtube_dl.utils.ExtractorError: 'youtube-dl' is not a valid URL. Set --default-search "ytsearch" (or run  youtube-dl "ytsearch:youtube-dl" ) to search YouTube

hans@hans-GA-78LMT-USB3:~$ [youtube] V38psI8WIvI: Downloading webpage
[youtube]: command not found
hans@hans-GA-78LMT-USB3:~$ [youtube] V38psI8WIvI: Downloading video info webpage
[youtube]: command not found
hans@hans-GA-78LMT-USB3:~$ [youtube] V38psI8WIvI: Extracting video information
[youtube]: command not found
hans@hans-GA-78LMT-USB3:~$ [youtube] V38psI8WIvI: Downloading js player vflvABTsY
[youtube]: command not found
hans@hans-GA-78LMT-USB3:~$ ERROR: Signature extraction failed: Traceback (most recent call last):
bash: syntax error near unexpected token `('
hans@hans-GA-78LMT-USB3:~$   File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1191, in _decrypt_signature

Command 'File' not found, did you mean:

  command 'file' from deb file
  command 'vile' from deb vile
  command 'zile' from deb zile
  command 'kile' from deb kile

Try: sudo apt install <deb name>

hans@hans-GA-78LMT-USB3:~$     video_id, player_url, s
video_id,: command not found
hans@hans-GA-78LMT-USB3:~$   File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1102, in _extract_signature_function

Command 'File' not found, did you mean:

  command 'file' from deb file
  command 'zile' from deb zile
  command 'kile' from deb kile
  command 'vile' from deb vile

Try: sudo apt install <deb name>

hans@hans-GA-78LMT-USB3:~$     res = self._parse_sig_js(code)
bash: syntax error near unexpected token `('
hans@hans-GA-78LMT-USB3:~$   File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1163, in _parse_sig_js

Command 'File' not found, did you mean:

  command 'file' from deb file
  command 'kile' from deb kile
  command 'vile' from deb vile
  command 'zile' from deb zile

Try: sudo apt install <deb name>

hans@hans-GA-78LMT-USB3:~$     jscode, 'Initial JS player signature function name', group='sig')
bash: syntax error near unexpected token `)'
hans@hans-GA-78LMT-USB3:~$   File "/usr/lib/python3/dist-packages/youtube_dl/extractor/common.py", line 796, in _search_regex

Command 'File' not found, did you mean:

  command 'kile' from deb kile
  command 'zile' from deb zile
  command 'vile' from deb vile
  command 'file' from deb file

Try: sudo apt install <deb name>

hans@hans-GA-78LMT-USB3:~$     raise RegexNotFoundError('Unable to extract %s' % _name)
bash: syntax error near unexpected token `('
hans@hans-GA-78LMT-USB3:~$ youtube_dl.utils.RegexNotFoundError: Unable to extract Initial JS player signature function name; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
youtube_dl.utils.RegexNotFoundError:: command not found
please: command not found
Error: no such file ":https://yt-dl.org/update"
Error: no such file "on"
Error: no such file "how"
Error: no such file "to"
Error: no such file "update."
Error: no such file "Be"
Error: no such file "sure"
Error: no such file "to"
Error: no such file "call"
Error: no such file "youtube-dl"
Error: no such file "with"
Error: no such file "the"
Error: no such file "flag"
Error: no such file "and"
Error: no such file "include"
Error: no such file "its"
Error: no such file "complete"
Error: no such file "output."
hans@hans-GA-78LMT-USB3:~$  (caused by RegexNotFoundError('Unable to extract \x1b[0;34mInitial JS player signature function name\x1b[0m; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.',)); please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
bash: syntax error near unexpected token `('
hans@hans-GA-78LMT-USB3:~$ hans@hans-GA-78LMT-USB3:~$ youtube-dl --verbose
hans@hans-GA-78LMT-USB3:~$: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] System config: []
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] User config: []
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] Custom config: []
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] Command-line args: ['--verbose']
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] Encodings: locale UTF-8, fs utf-8, out UTF-8, pref UTF-8
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] youtube-dl version 2018.03.14
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] Python version 3.6.5 (CPython) - Linux-4.15.0-33-generic-x86_64-with-Ubuntu-18.04-bionic
bash: syntax error near unexpected token `('
hans@hans-GA-78LMT-USB3:~$ [debug] exe versions: ffmpeg 3.4.4-0ubuntu0.18.04.1, ffprobe 3.4.4-0ubuntu0.18.04.1, phantomjs 2.1.1, rtmpdump 2.4
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ [debug] Proxy map: {}
[debug]: command not found
hans@hans-GA-78LMT-USB3:~$ Usage: youtube-dl [OPTIONS] URL [URL...]
Usage:: command not found
hans@hans-GA-78LMT-USB3:~$ 
