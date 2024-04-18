# Musicbox Help

All Bot commands are executed from the IRC channel.

* Server: irc.rizon.net
* Channel: #randommusic
* [Cytube Stream](https://cytu.be/r/MusicBox)

To add a song, paste a youtube, bandcamp or soundcloud URL.

## Commands

`.commands|.help` Show the url to this readme.

`.start` Start the stream.

`.stop` Stop the stream.

`.yt|.you|.youtube <query>` Query youtube for a song and automatically add it to the playlist.

`.soundcloud <query>` Query soundcloud for a song and automatically add it to the playlist.

`.skip|next` Skip the currently playing song.

`.search <query>` Search for songs in the database.

`.np` Show the currently playing song.

`.yn` Flip a coin.

`.8ball` Ask the magic 8 ball a question.

`.stats` Overall statistics about songs in the database.

`.random` Add a random song to the playlist.

`.random-<nick>` Add a random songs from a specific nick to the playlist.

`.random^<int>-<nick>` Add multiple random songs from a specific nick to the playlist.

`.random-!<nick>` Add a random song to the playlist but exclude a specific nick.

`.filter-<nick>` Let the stream only play songs from a specific nick.

`.filter-!<nick>` Let the stream not play songs from a specific nick.

`.filter on|off` Turn the filter on or off.

`.flag <url>` Flag a URL. **(Only Admins)**

`.unflag <url>` Unflag a url. **(Only Admins)**

`.band <name>` Show information about an artist from last.fm.

`.link <nick>` If you are using multiple nicks you can link them together.

`.unlink <nick>` Unlink one of your nicks.

`.ustat [nick]` Get statistics about yourself or about a specific nick.

`.ulist [nick]` Get a list of links from yourself or from a specific nick.

`.prune <url>` Remove a link from your list.

`.unprune <url>` Un-remove a link from your list.

`.lastfm-recent <username>` Show the last track scrobbled by a last.fm user.

`.img <url>` Asciify an image from URL.

`.leaderboard` Show the current leaderboard.
