---
layout: post
title:  Properties, Methods and Events of Syncfusion ejMediaPlayer Widget
description: API reference for ejMediaPlayer
documentation: ug
platform: js-api
keywords: mediaplayer, ejMediaPlayer, syncfusion, medaiplayer api 
---

# ejMediaPlayer

Media player is a HTML5 component that is used to embed web videos, YouTube, and audio files in web pages.


#### Syntax

{% highlight javascript %}

$(element).ejMediaPlayer(options)

{% endhighlight %}

#### Example



{% highlight html %}

<div id="basicPlayer"></div>

<script>
// Create Media Player
$("#basicPlayer").ejMediaPlayer();
</script>

{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.globalize.js

* module:ej.data.js

* module:ej.scroller.js

* module:ej.touch.js

* module:ej.button.js

* module:ej.checkbox.js

* module:ej.togglebutton.js

* module:ej.slider.js

* module:ej.waitingpopup.js

* module:ej.listview.js

* module:ej.listbox.js

* module:ej.mediaplayer.js


N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.


## Members







### autoPlay `boolean`
{:#members:autoplay}


Enables/disables the player automatically.




### Default value







* true







{% highlight html %}
 
<div id="basicPlayer"></div>

<script>
//To set autoPlay API during initialization
   $("#basicPlayer").ejMediaPlayer({ autoPlay:false });
</script>

{% endhighlight %}






### autoHide `boolean`
{:#members:autohide}



Hides the toolbar and header content when mouseout of the content area. The default value is true.




### Default value







* true







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set autoHide API during initialization
 $("#basicPlayer").ejMediaPlayer({ autoHide:false });
</script>

{% endhighlight %}







### autoHideTime `number`
{:#members:autohidetime}

Specifies the duration (seconds) when toolbar and content need to be hidden.




### Default value








* 3







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set autoHideTime API during initialization
        $("#basicPlayer").ejMediaPlayer({ autoHideTime:5 });
</script>

{% endhighlight %}







### contentType `string|enum`
{:#members:contenttype}


Sets the content type of the player such as video or audio.




### Default value







* "video"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
////To set contentType API during initialization
        $("#basicPlayer").ejMediaPlayer({contentType:"audio" });
</script>

{% endhighlight %}







### cssClass `string`
{:#members:cssclass}


Sets the root CSS class for media player theme, which is used to customize alignment, color, and more.




### Default value








* ""







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
 //To set cssClass API during initialization 
        $("#basicPlayer").ejMediaPlayer({ cssClass:"gradient-lime" });
</script>

{% endhighlight %}






### disableKeys `boolean`
{:#members:disablekeys}


Enables/disables keyboard shortcuts using disableKeys property. It is false, by default.




### Default value








* false







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set disableKeys API during initialization 
        $("#basicPlayer").ejMediaPlayer({ disableKeys:true });
</script>

{% endhighlight %}






### forwardTime `number`
{:#members:forwardtime}


Forwards the current audio/video source of the media player from the current time to the specified time (seconds).




### Default value








* 10s







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set forwardTime API during initialization 
        $("#basicPlayer").ejMediaPlayer({ forwardTime : 30 });
</script>

{% endhighlight %}






### locale `string`
{:#members:locale}


Sets the language for the media player control using locale property. 




### Default value








* "en-US"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
 //To set locale API during initialization  
        $("#basicPlayer").ejMediaPlayer({  locale: "en-US"});
</script>

{% endhighlight %}







### height `string`
{:#members:height}


Specifies the height of the media player.




### Default value








* "100%"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
  //To set height API during initialization 
        $("#basicPlayer").ejMediaPlayer({ height: "400px" });
</script>

{% endhighlight %}







### mute `boolean`
{:#members:mute}


Mutes the media player.





### Default value







* false







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
 //To set mute API during initialization  
        $("#basicPlayer").ejMediaPlayer({ mute:true });
</script>

{% endhighlight %}






### playSpeed `number`
{:#members:playspeed}


Returns the speed of the audio/video player.




### Default value







* 1







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
  //To set playSpeed API during initialization 
        $("#basicPlayer").ejMediaPlayer({ playSpeed:2 });
</script>

{% endhighlight %}






### repeat `boolean`
{:#members:repeat}


Enables/disables repeat functionality of the play list.




### Default value







* false








{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
  //To set repeat API during initialization 
        $("#basicPlayer").ejMediaPlayer({ repeat: true});
</script>

{% endhighlight %}







### renderMode `string|enum`
{:#members:rendermode}


The three rendering layouts in the media player are basic, advanced, and mobile.


*ej.MediaPlayer.RenderMode.Basic
*ej.MediaPlayer.RenderMode.Advanced
*ej.MediaPlayer.RenderMode.Mobile





### Default value








* "basic"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set renderMode API during initialization 
        $("#basicPlayer").ejMediaPlayer({ renderMode: "mobile"});
</script>

{% endhighlight %}








### rewindTime `number`
{:#members:rewindtime}


Rewinds the current audio/video source of the media player from the current time to the specified time (seconds).




### Default value







* 10s







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
 //To set rewindTime API during initialization 
        $("#basicPlayer").ejMediaPlayer({  rewindTime : 30 });
</script>

{% endhighlight %}






### showPlaylist `boolean`
{:#members:showplaylist}


Shows the play list panel.




### Default value







* false







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set showPlaylist API during initialization 
        $("#basicPlayer").ejMediaPlayer({ showPlaylist: true });
</script>

{% endhighlight %}






### source `object|Array`
{:#members:source}

Consist of the following items.

* url: Specifies the URL link of the required file.
* title: Specifies the title of the required file.
* posterUrl: Specifies the background image for the required file.
* author: Specifies the name of the author.




### Default value






* []







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set source API during initialization 
        $("#basicPlayer").ejMediaPlayer({  source: [
                        {
                            "url": "http://files2.syncfusion.com/Videos/samples/Managing+Static+Files+in+ASP.NET+Core%2C+presented+by+Ugo+Latt.mp4",
                            "title": "Managing Static Files in ASP.NET",
                            "posterUrl": "images/media player/SFFlatLicense.png",
                            "author": "syncfusion"
                        }
                       ]
                    });
</script>

{% endhighlight %}







### playlistTitle `string`
{:#members:playlisttitle}

Shows the title of the play list panel.




### Default value







* "Playlist"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
 //To set playlistTitle API during initialization 
        $("#basicPlayer").ejMediaPlayer({ playlistTitle: "Syncfusion" });
</script>

{% endhighlight %}






### showPoster `boolean`
{:#members:showposter}


Shows/hides the poster by setting showPoster property. It is set to true, by default.




### Default value







* true








{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set showPoster API during initialization 
        $("#basicPlayer").ejMediaPlayer({ showPoster:false});
</script>

{% endhighlight %}






### showTitle `boolean`
{:#members:showtitle}


Shows/hides the title by setting the showTitle property. It is set to true, by default.



### Default value







* true







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set showTitle API during initialization 
 $("#basicPlayer").ejMediaPlayer({ showTitle:false });
</script>

{% endhighlight %}






### shuffle `boolean`
{:#members:shuffle}


Enables/disables the shuffle functionality of the play list.




### Default value







* false







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set shuffle API during initialization 
        $("#basicPlayer").ejMediaPlayer({  shuffle: true});
</script>

{% endhighlight %}






### toolbarHeight `string`
{:#members:shuffle}


Specifies the height of the toolbar.




### Default value







* "45px"







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set toolbarHeight API during initialization 
        $("#basicPlayer").ejMediaPlayer({ toolbarHeight:"50px"});
</script>

{% endhighlight %}






### volume `number`
{:#members:volume}

Defines the volume (0-100) of the player.




### Default value







* 50







{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set volume API during initialization 
        $("#basicPlayer").ejMediaPlayer({ volume: 60});
</script>

{% endhighlight %}






### width `string`
{:#members:width}


Specifies the width of the media player.



### Default value








* "100%"








{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
//To set width API during initialization 
$("#basicPlayer").ejMediaPlayer({width: "700px"});
</script>

{% endhighlight %}






## Methods





### exitFullScreen()
{:#methods:exitfullscreen}

Used to exit the full screen of the player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>

<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
playerObj.exitFullScreen(); // exit full screen
</script>

{% endhighlight %}







### getCurrentMediaIndex()
{:#methods:getcurrentmediaindex}


Returns the current index of the play list..


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.getCurrentMediaIndex(); // returns current index of play list
</script>

{% endhighlight %}







### getCurrentTime()
{:#methods:getcurrenttime}

Returns the current playing time (seconds).

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.getCurrentTime(); // returns current playing time. 
</script>

{% endhighlight %}







### getCurrentMediaType
{:#methods:getcurrentmediatype}


Returns the following types of current source.

* ej.MediaPlayer.Types.Audio
* ej.MediaPlayer.Types.Video
* ej.MediaPlayer.Types.YouTube

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.getCurrentMediaType(); // returns current media type
</script>

{% endhighlight %}








### getDuration()
{:#methods:getduration}

Returns the whole duration (seconds) of the current source (video/audio).

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.getDuration(); // returns duration of current source
</script>


{% endhighlight %}







### getMediaSpeed()
{:#methods:getmediaspeed}


Returns the media speed.


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
playerObj.getMediaSpeed(); // returns speed of the media
</script>



{% endhighlight %}








### getVolume()
{:#methods:getvolume}

Returns the volume of the player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.getVolume(); // returns player volume
</script>

{% endhighlight %}







### hidePlaylist()
{:#methods:hideplaylist}


Hides the play list panel.


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
playerObj.hidePlaylist(); // hides the play list
</script>
{% endhighlight %}







### makeFullScreen()
{:#methods:makefullscreen}

Enables full screen mode for the player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
playerObj.makeFullScreen(); // make full screen
</script>
{% endhighlight %}







### mute()
{:#methods:mute}


Allows muting the media player.


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.mute(); 
</script>

{% endhighlight %}






### next()
{:#methods:next}


Allows playing the next audio/video source of the media player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.next(); 
</script>

{% endhighlight %}







### pause()

{:#methods:pause}

Allows pausing the current audio/video source of the media player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.pause(); 
</script>

{% endhighlight %}






### previous()
{:#methods:previous}



Plays the previous audio/video source of the media player.


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
playerObj.previous(); 
</script>

{% endhighlight %}






### play()

{:#methods:play}

Plays the current audio/video source of the media player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.play(); 
</script>

{% endhighlight %}






### stop()
{:#methods:stop}


Stops the current audio/video source of the media player.

#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.stop(); 
</script>

{% endhighlight %}






### unmute()
{:#methods:unmute}


Allows to unmute the media player.


#### Example



{% highlight html %}
 
<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer();
// Create Media Player instance
var playerObj = $("#basicPlayer").data("ejMediaPlayer");
 playerObj.unmute(); 
</script>

{% endhighlight %}






## Events





### onActionBegin
{:#events:onactionbegin}




Triggers when any action begins.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onActionBegin: function(args){}
});
</script>
            

{% endhighlight %}




### onActionComplete
{:#events:onactioncomplete}




Triggers when any action ends.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onActionComplete: function(args){}
});
</script>
            

{% endhighlight %}




### onTogglePlaylist
{:#events:ontoggleplaylist}




Triggers when showing/hiding the play list (through showPlaylist API).




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    showPlaylist: true,
    onTogglePlaylist: function(args){}
});
</script>
            

{% endhighlight %}




### onPlaying
{:#events:onplaying}




Triggers while playing current media source.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onPlaying: function(args){}
});
</script>
            

{% endhighlight %}



### onRepeat
{:#events:onrepeat}




Triggers on toggling repeat functionality. Get the enabled or disabled repeat status using  "isRepeat" parameter.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onRepeat: function(args){}
});
</script>
            

{% endhighlight %}



### onShuffle
{:#events:onshuffle}




Triggers on toggling shuffle functionality. Get the enabled or disabled shuffle status using isShuffle" parameter.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onShuffle: function(args){}
});
</script>
            

{% endhighlight %}





### onMediaComplete
{:#events:onmediacomplete}




Triggers when the player successfully reaches the end of the current media source.




#### Example



{% highlight html %}
 

<div id="basicPlayer"></div>
<script>
$("#basicPlayer").ejMediaPlayer({
    onMediaComplete: function(args){}
});
</script>
            

{% endhighlight %}