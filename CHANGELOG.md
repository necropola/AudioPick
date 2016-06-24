# CHANGELOG

### AudioPick-0.1.4 - 2016-05-17
- only call `getUserMedia()` on a site (once) when a call to `setSinkId` actually fails. This should greatly reduce the number of sites added to teh list of microphone exceptions.  
- change `browser_action` into `page_action`
- use *declarative content* to only enable the `page_action` when certain conditions (HTTPS video/audio) are met on the content page
- immediately commit changes to the popup device list (commit button removed)
- remember the last temporary `sink_no` choice of a content page when creating the popup device list for it
