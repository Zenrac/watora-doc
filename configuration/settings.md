---
description: Explanation to set custom settings for the bot.
---

# Settings

{% hint style="info" %}
You can use `settings`to display current Watora's settings.
{% endhint %}

## Global Settings

### Set a custom prefix on your server

To set a custom prefix you have to use`prefix`

| Usage | Help |
| :--- | :--- |
| **`prefix change [new_prefix]`** | Allows to set \[new\_prefix\] as the new server prefix. |
| **`prefix now`** | Displays the current server prefix. |
| **`prefix reset`** | Resets the server prefix to the global one. |

### Set a custom language on your server

To set a custom language you have to use `language`

| Usage | Help |
| :--- | :--- |
| **`language [lang]`** | Allows to set \[lang\] as the new server language. |
| **`language list`** | Displays available language list. |

## Music Settings

### Set a custom default volume

{% hint style="info" %}
Each time Watora disconnects herself from a voice channel, the player volume is reset to the default volume \(by default, 50%\).
{% endhint %}

To set a custom default volume you have to use `defvolume`

| Usage | Help |
| :--- | :--- |
| **`defvolume set [number]`** | Sets the default volume to \[number\]. |
| **`defvolume now`** | Displays the current default volume. |
| **`defvolume reset`** | Resets Watora's default volume. |

### Set a custom autoleave time

{% hint style="info" %}
By default, Watora's auto-disconnects herself from the voice channel if she's alone or not playing anything since an autoleave time \(by default 3 minutes\).
{% endhint %}

To set a custom autoleave time you have to use `autoleave`

| Usage | Help |
| :--- | :--- |
| **`autoleave set [second]`** | Edits Watora's time before leaving the voice channel for inactivity to \[second\] |
| **`autoleave never`** | Disables Watora's auto-disconnect function for inactivity. |
| **`autoleave reset`** | Resets Watora's time before leaving the voice channel for inactivity. |
| **`autoleave now`** | Displays Watora's current time before leaving the voice channel for inactivity. |

### Set a custom channel or disable auto now playing messages

{% hint style="info" %}
By default, an auto now playing message is sent when a new song starts. It's sent in the same channel than where you called Watora.
{% endhint %}

To set a custom channel for Now Playing or to disable them you have to use `npmsg`

| Usage | Help |
| :--- | :--- |
| **`npmsg set [channel]`** | Sets a default channel for auto now playing messages. |
| **`npmsg never`** | Disables now playing messages at the beginning of new song. |
| **`npmsg reset`** | Resets Watora's setting about auto now playing messages at the beginning of new songs. |
| **`npmsg now`** | Displays Watora's current setting about auto now playing messages at the beginning of new songs. |



