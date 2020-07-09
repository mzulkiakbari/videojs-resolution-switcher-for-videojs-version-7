I using videojs version 7.7.4.

How to install:

Insert Stylesheet before head tag.
<link href="videojs-resolution-switcher.css" rel="stylesheet">

Insert this script before body tag and below video tag.
<script src="videojs-resolution-switcher.js"></script>


How to usage:

var Player = videojs('YOUR_VIDEO_ID',{
  "controls" : true,
  "autoplay" : true,
  "preload" : "metadata",
  "width" : "100%",
  "height" : "auto",
  sources : [
    { src : 'http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4', type : 'video/mp4', label : 'SHK', res: 'SHK'},
    { src : 'http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4', type : 'video/mp4', label : 'HK', res: 'HK'},
    { src : 'http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4', type : 'video/mp4', label : 'HD', res: 'HD'}
  ],
});
videojs('YOUR_VIDEO_ID').videoJsResolutionSwitcher();
