# obs-youtube-playlist-title
Show title of current song playing in a youtube playlist. 


# Usage
This page works on youtube playlists. So you'll need to start by getting the url. Let's take the swolejams playlist https://www.youtube.com/watch?v=I9kC5ZxDQ9E&list=PL8dcsJNXFe0Qndwgrrax091jhU7xNrKhG&index=1 (dmca free music for you!) as an example.

You will need to take all the query parameters (everything after `?`) and append them to https://swolekat.github.io/obs-youtube-playlist-title/? 

In our example it will look like https://swolekat.github.io/obs-youtube-playlist-title?v=I9kC5ZxDQ9E&list=PL8dcsJNXFe0Qndwgrrax091jhU7xNrKhG&index=1

If you want to change the volume via the url you can append `&volume=num` where num is a value from 0 to 100 inclusive.

If you want to show the video via the url you can append `&video=true`. The video will take up 100% of the browser.

You'll then take this url and put it in OBS as a browser source. The size doesn't matter too much, but I'd just make it 1920x1080 in case of a long title.

You may want to change how it looks. You'll need to know some css. There are two classes `.title` and `.author`. In the `Custom CSS` section of the browser source you can put your stuff here.

For example, let's say you want to change the text to white. You would write this:
```css
.title {
    color: #fff;
}

.author {
    color: #fff;
}
```

# Troubleshooting
* If the music is playing and you want it to stop, make sure you check the `Shutdown source when not visible` checkbox

# Contact
If you have any questions or suggestions please contact me on my [twitch stream](https://www.twitch.tv/swolekat). 
