# itunes2volumio
Changes iTunes M3U playlist to Volumio playlist with function of changing iTunes path to NAS network path

Instructions:

Run this command in directory of Python script, with auto SSH transfer to Volumio instance (must setup SSH keys for passwordless access):

py volumio.py "filename.m3u" itunes | ssh volumio@[IPADDRESS] "cat > /data/playlist/[NAMEOFPLAYLIST]

Feel free to edit "NASlocation" and "iTunesPrefix" to your local NAS drive path and iTunes library prefix, which will result in perfect file names uploaded directly to Volumio.
