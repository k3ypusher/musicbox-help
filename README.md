# Musicbox Help

All bot commands are executed from the IRC channel.

* Server: irc.rizon.net
* Channel: #randommusic
* [Cytube Stream](https://cytu.be/r/MusicBox)
* [Last.fm Scrobbles](https://www.last.fm/user/MusicBoxIRC)
* [Top 50 Leaderboard](https://musicbox.gamefiar.com)
* [We also have an API](https://github.com/ftab/musicbox-api)

To add a song, simply paste a YouTube, Bandcamp or SoundCloud URL.

**Please note** if you want to share a link that is **NOT** a song, start your message with a `#` so it doesn't get added to the stream.

## Commands

### `.commands|.help|!help`

Show the link to this README.

### `.start` and `.stop`

Start or stop the stream on Cytube.

Usually the stream is always running. Just after restarting the bot, the stream has to be started manually once.
There is actually no reason to stop the stream, but who knows.

### `.yt|.you|.youtube <query>`

Query YouTube for a song and automatically add it to the playlist on Cytube.

### `.soundcloud <query>`

Query SoundCloud for a song and automatically add it to the playlist on Cytube.

### `.random`

Add a random song from the bot's database to the playlist on Cytube.

This command has a few complicated variants:

- `.random-<nick>` will add a random song **only** from a specific user.
- `.random-!<nick>` will add a random song **except** from a specific user.
- `.random^<int>-<nick>` will add multiple random songs from a specific user.

### `.filter on|off`

Since the stream automatically adds new songs to the playlist when nothing gets posted by users, you can set a filter to include or exclude specific user submissions.

Before you can turn the filter on, specify at least:

- `.filter-<nick>[,nick...]` which users should be **included** or
- `.filter-!<nick>[,nick...]` which users should be **excluded**.

Remember to turn the filter off after listening.

### `.np`

Show which song is currently playing on Cytube.

### `.source`

Show which user added the currently playing song.

### `.skip|.next`

Skip the currently playing song on Cytube.

### `.search <query>`

Search for songs in the bot's database.

The bot will generate a [paste.ee](https://paste.ee) link for you, which contains the search results.

### `.stats`

Show the overall statistics about songs in the bot's database.

### `.leaderboard`

Generates a [paste.ee](https://paste.ee) link for you, which contains the current leaderboard.

We also have a [graphical leaderboard](https://musicbox.gamefiar.com) of the top 50 submitters.

### `.ustat [nick]`

Show statistics about songs a user has posted.

If no nick is passed to the command, the bot will show statistics for yourself.

### `.ulist [nick]`

Let the bot generate a [paste.ee](https://paste.ee) link for you, which contains all songs a user has posted.

If no nick is passed to the command, the bot will generate a link for all your posted songs.

### `.prune <url>` and `.unprune <url>`

You can control which songs should appear on your ulist.

Pruning your ulist will not affect the songs in the database.

### `.flag <url>` and `.unflag <url>`

Flag or unflag URLs in the bot's database.

**These commands are only available to Admins!**

### `.link <primarynick>` and `.unlink <primarynick>`

If you are using alternative nicks on IRC, you can link each of them to your primary nick.

### `.band <artist>`

The bot will query the last.fm API to show information about an artist.

### `lastfm-recent <username>`

The bot will show the latest scrobbled song of a last.fm user.

### `.yn [string]`

Flip a coin, the bot will answer with YES or NO.

### `.8ball [string]`

Ask the magic 8 ball a question.

### `.choose <string>`

The bot will pick a choice for you if you have trouble to decide on something.

Just pass a list of things you are uncertain about, separated by any non-word character like commas maybe. (Spaces will not work).

### `.img <url>`

The bot will asciify an image from an URL for you.
