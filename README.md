# heroku-buildpack-youtube-dl

A Heroku buildpack that downloads and installs the latest version of youtube-dl.

**youtube-dl requires [Python](http://www.python.org) version 2.6, 2.7, or 3.2+.**

Scripts shamelessly copied from jonathanong/heroku-buildpack-ffmpeg-latest & modified for youtube-dl.

# Usage

Add the following URL to your app's buildpacks:
```
https://github.com/RFoley/heroku-buildpack-youtube-dl.git
```

youtube-dl can then be accessed using the command line

e.g. using Ruby:
```ruby
IO.popen("youtube-dl -q -o - URL_HERE")
```

You can find the docs for youtube-dl [here](https://ytdl-org.github.io/youtube-dl/index.html).