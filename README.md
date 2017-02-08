# webfront
Dawn's web front end (desktop and mobile via Firefox and Chrome).  We think that ours is a more efficient, resilient web front end system because of its heavy emphasis on native browser based p2p solutions like webrtc and webtorrent.  Expect us to devote time and money to continue to pursue solutions that implement simple, repeatable p2p techniques across our stack.  This folder currently contains just some javascript for our front end.

In terms of the overall design of the interactions of components of the Dawn network, here goes:

User -> Dawn

#1 User Uploads Content by seeding a webtorrent from their browser using drag and drop 
#2 Validator/Seed Network Ensures >=4x Replication & geo-distribution
#3 Validators run periodic checks on content to ensrue that it is the same content they have a hash for
#4 User is taken to the share page for their new content

Dawn -> User

#1 User clicks a link that begins a file load either of .md or one of the many other media types webtorrent can easily handle. This includes some novel filetypes of our own, which generally resemble TOML when possible.
#2 User's browser streams from Dawn's web seeds and displays the content according to filetype and tags

User <---> User

* WebRTC Video
* WebRTC Audio
* WebRTC Chat/IM
* WebTorrent COntent
