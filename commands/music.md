---
description: Help with music commands.
---

# Music

{% hint style="info" %}

**Reminder :**

`command (optional) [required] [choice|choice_2]`

* Parameters between parenthesis are optional.
* Parameters between square brackets are required.
* Parameters separated by vertical bars means that you have to choose one of them. 
* Any characters outside parenthesis and brackets are supposed to be written.

| Usage | Help |  |
| :--- | :--- | :--- |
| `join (voice_channel)` | Summons Watora into your voice channel or into the specified one. |  |
| `np` | Returns some information about the current song. |  |
| \*\*\`play \[key\_words | URL\]\`\*\* | Enqueues a song with an URL or keywords. Can also enqueue a stream or a radio. |
| `queue (page)` | Displays the current song queue. |  |
| `search (service)[query](--full)` | Searches multiple videos at once with the selected parameters. You can add one of them to the queue. If no service are specified, YouTube is selected by default.  _Available services : YouTube, SoundCloud_ |  |
| `skip` | Skips the current song. |  |
| `forceskip (queue_position)` | Skips the current song without needing to vote. If you specify a queue position, skips every song until the chosen position. |  |
| `replay` | Enqueues the current song. |  |
| `previous` | Enqueues the previous song. |  |
| `replaynow` | Immediately replays the current song. |  |
| `previousnow` | Immediately replays the last song. |  |
| `stop` | Stops the player and clears the queue. |  |
| `repeat` | Enables or disables the repeat mode. |  |
| `pause` | Pauses the currently playing song. |  |
| `volume ((+/-)[value])` | Sets the playback volume. Accepted values are from 0 to 1000. Putting `+` or`-` before the volume will make the volume change relative to the current volume. If you don't specify any new volume, returns the current volume. |  |
| \*\*\`playnow \[key\_words | URL\]\`\*\* | Immediately plays a song. |
| \*\*\`playnext \[key\_words | URL\]\`\*\* | Enqueues a song to the first position of the queue. |
| `clear` | Clears the current queue. |  |
| `promote ([song_position] (after_position))` | Moves a song by specifying its queue index. If you don't specify an after position, moves it to the first position of the queue. If you don't specify a song either, it will promotes the last song of queue to the first position of the queue. |  |
| `shuffle` | Shuffle the queue. |  |
| `remove ([first_position] (second_position))` | Removes a song from the queue. If you don't specify any position, removes the last song in queue. Otherwise remove a song based on its position in queue. You can specify a second position to remove every song between the two positions. |  |
| `moveto (+/-) [time]` | Moves the song to a specific moment. You can either specify a time in hh:mm:ss format or add a relative time like + 30 to move 30 secondes forward. |  |
| \*\*\`lyrics \(key\_words | URL\)\`\*\* | Displays the lyrics of a song. If you don't specify any url or keywords, it displays the current song lyrics. |
| `bassboost (level)` | Changes the player's bass frequencies up to 4 levels. `OFF, LOW, MEDIUM, HIGH, INSANE.`You can use the equalizer to make adjustments as you want. Displays the current setting if you don't specify any level. |  |
| `equalizer ([band] [gain])` | Manages an equalizer with 15 bands. Valid values are from -0.25 to 1. -0.25 means that the given frequency is completely muted and 0.25 means it is doubled. Use reactions to move the cursor and edit gains interactively. You can press the circle to reset the equalizer. Otherwise you can specify a band and a gain to edit it quickly. |  |
| \*\*\`radio \[play | list\]\`\*\* | Radio commands management. |
| `radio play` | Adds a radio from the known radios to the queue to be played. _For other radios, you'll have to play them manualy with_`play` |  |
| `radio list` | Displays the list of my available radio stations. |  |
| `pl` | This command has [her own page here](../features/autoplaylists.md) |  |

