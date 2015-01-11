musicbox-webclient
==================

Just a visual reworking of Wouter van Wyks PiMusicbox webclient for MPD, basically just moving a few elements around using jquery appendTo so you get the best layout in both large screen browsers and mobile devices, css tweaks for a darker theme..

Added from original webclient
- independently scrollable playlist and song queue divs
- volume slider movies to header on small screens for easy access
- now playing moves to side panel on large view and removed from menu as redundant
- play controls now always show in footer on big screen, again for easy access
- slightly cleaned up queue layout, just personal but breaking into albums confused me, also no need to show album for each song on small viewspace. Also I made it easier to see which is the artist and album etc, used to be confusing
- added right side settings panel in header to free up some space from Now Playing panel (Work In Progress!)
- colour toggles on random/repeat etc to see when on 


To Do
- I have hardcoded links to my other Musicboxs' on the same network so I can easily switch between them, this should be configurable through settings ie can add the IP / name in settings 
- default open current playlist when open on new device
- get Random button to not change tracks when set to on

Need to create these symlinks to make things work after replacing the webclient
	ln -s /boot/config/radiostations.js /opt/webclient/js/radiostations.js
	ln -s /usr/local/lib/python2.7/dist-packages/mopidy/http/data /opt/webclient/mopidy

Probably broke some other things while tinkering..