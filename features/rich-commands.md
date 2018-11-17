---
description: Explains what is a rich command. And her differences with a basic command.
---

# Rich Commands

## Rich Commands Attributes

Rich commands are an useful part of Watora's command creating unlimited possibilities.

### Image URLs are automatically hidden

![](../.gitbook/assets/capture-du-2018-11-17-17-18-36.png)

{% hint style="info" %}
You can use this feature to create cool custom commands or welcome messages
{% endhint %}

### There are variables

By writing a variable between curly brackets, you can get a real value.

![Here, I get my username and my avatar url](../.gitbook/assets/image%20%2811%29.png)

{% hint style="info" %}
`author.avatar_url`gives a link, as `choice`is a Rich Command, the link is hidden.
{% endhint %}

#### Availables variables and its attributes

{% hint style="info" %}
in `author.name`**author** is a **variable**, and **name** an **attribute**
{% endhint %}

<table>
  <thead>
    <tr>
      <th style="text-align:left">Variable</th>
      <th style="text-align:left">Attributes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>message</code></b>
      </td>
      <td style="text-align:left">
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.attachments">attachments</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.author">author</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.content">content</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.created_at">created_at</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.edited_at">edited_at</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.guild">guild</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.embeds">embeds</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.id">id</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.jump_url">jump_url</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Message.tts">tts</a>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b><code>author</code></b>
        </p>
        <p><b><code>user</code></b>
        </p>
        <p><b><code>member</code></b>
        </p>
        <p><b><code>random_member</code></b>
        </p>
      </td>
      <td style="text-align:left">
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.voice">voice</a>
          <br
          /><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.color">color</a>
          <br
          /><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.bot">bot</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.avatar_url">avatar_url</a>
          <br
          /><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.top_role">top_role</a>
          <br
          /><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.display_name">display_name</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.roles">roles</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.joined_at">joined_at</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.default_avatar_url">default_avatar_url</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.id">id</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.mention">mention</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.discriminator">discriminator</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.name">name</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.nick">nick</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.guild">guild</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.is_avatar_animated">is_avatar_animated</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Member.status">status</a>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>channel</code></b>
      </td>
      <td style="text-align:left">
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.is_nsfw">nsfw</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.members">members</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.slowmode_delay">slowmode_delay</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.guild">guild</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.name">name</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.id">id</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.category">category</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.created_at">created_at</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.TextChannel.position">position</a>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b><code>guild</code></b>
        </p>
        <p><b><code>server</code></b>
        </p>
      </td>
      <td style="text-align:left">
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.name">name</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.afk_timeout">afk_timeout</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.afk_channel">afk_channel</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.id">id</a>
          <br
          /><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.region">region</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.owner_id">owner_id</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.unavailable">unavailable</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.mfa_level">mfa_level</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.features">features</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.splash_url">splash_url</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.channels">channels</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.me">me</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.icon_url">icon_url</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.shard_id">shard_id</a>
        </p>
        <p><a href="https://discordpy.readthedocs.io/en/rewrite/api.html#discord.Guild.created_at">created_at</a>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>current</code></b>
      </td>
      <td style="text-align:left">
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">artwork</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">author</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">can_seek</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">duration</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">identifier</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">requester</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">stream</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">thumbnail</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">track</a>
        </p>
        <p><a href="https://github.com/Devoxin/Lavalink.py/blob/master/lavalink/AudioTrack.py">uri</a>
        </p>
      </td>
    </tr>
  </tbody>
</table>{% hint style="warning" %}
`current`only works if there's a current song.
{% endhint %}

{% hint style="info" %}
`random_member`is a random member taken from the current guild.
{% endhint %}

#### Variable without attributes

| Variable | Documentation |
| :--- | :--- |
| **`day`** | Returns the current day's number. |
| **`month`** | Returns the current month's number. |
| **`year`** | Returns the current year's number. |
| **`server_members`** | Returns the number of member in the current guild. |

**Example :**

![](../.gitbook/assets/image%20%285%29.png)

#### Specials

<table>
  <thead>
    <tr>
      <th style="text-align:left">Number</th>
      <th style="text-align:left">Documentation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>(nb1)~(nb2)</code></b>
      </td>
      <td style="text-align:left">
        <p>Generates a random number between nb1 and nb2.</p>
        <p><em>If not specified, nb1 is 0, and nb2 is 100.</em>
        </p>
      </td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
Using `{~}` do the same thing than using`{0~100}`
{% endhint %}

**Example :**

![](../.gitbook/assets/image%20%2812%29.png)

### You can call a command

By using `>>>`you can specify that the following word is a command.

**Example :**

![The choice command chosen to start the flip command](../.gitbook/assets/image%20%283%29.png)

###  **You can even call several commands**

By adding `&&`between your commands, you can start several commands at the same time.

{% hint style="info" %}
It's not exactly at the same time, commands are started in order, starting from the beginning.
{% endhint %}

**Example :**

![Doing both commands](../.gitbook/assets/image%20%288%29.png)

## What's the point of Rich Commands ?

* Custom Commands are [Rich Commands](rich-commands.md).
* Welcome and Goodbye messages are [Rich Commands](rich-commands.md).
* You can call a command in Custom Command, see [Custom Commands page](custom-commands-1.md) to get started.
* You can even mix several commands into one [Custom Command.](custom-commands-1.md)

