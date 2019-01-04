# Settings

{% hint style="info" %}
You can use`settings`to display current Watora's settings.
{% endhint %}

## Global Server Settings

### Set a custom prefix

{% hint style="info" %}
Discord auto-deletes your useless spaces at the end of your messages.

You have to litteraly write square brackets`[]`in your new prefix to keep your spaces.
{% endhint %}

To set a custom prefix you have to use`prefix`

| Usage | Help |
| :--- | :--- |
| **`prefix change [new_prefix]`** | Allows to set \[new\_prefix\] as the new server prefix. |
| **`prefix now`** | Displays the current server prefix. |
| **`prefix reset`** | Resets the server prefix to the global one. |

### Set a custom language

To set a custom language you have to use `language`

| Usage | Help |
| :--- | :--- |
| **`language [lang]`** | Allows to set \[lang\] as the new server language. |
| **`language list`** | Displays available language list. |

### Set a Welcome message

To set a welcome message you have to use `welcome`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>welcome [text] (| [text2] | [text3]...)</code></b>
      </td>
      <td style="text-align:left">
        <p>Enables a message that will be sent to the channel when someone join the
          server. You can specify serveral text separated by a vertical bar and one
          will be randomly sent.</p>
        <p><em></em><a href="../features/rich-commands.md"><em>This command is a Rich Command</em></a><em></em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>welcome off</code></b>
      </td>
      <td style="text-align:left">Disables the welcome message on the channel.</td>
    </tr>
  </tbody>
</table>### Set a Goodbye message

To set a goodbye message you have to use `goodbye`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>goodbye [text] (| [text2] | [text3]...)</code></b>
      </td>
      <td style="text-align:left">
        <p>Enables a message that will be sent to the channel when someone leaves
          the server. You can specify serveral text separated by a vertical bar and
          one will be randomly sent.</p>
        <p><em></em><a href="../features/rich-commands.md"><em>This command is a Rich Command</em></a><em></em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>goodbye off</code></b>
      </td>
      <td style="text-align:left">Disables the goodbye message on the channel.</td>
    </tr>
  </tbody>
</table>### Set one or serveral auto roles

{% hint style="info" %}
Auto roles are given when an use join the server.
{% endhint %}

To set one or several auto roles you have to use `autorole`

| Usage | Help |
| :--- | :--- |
| **`autorole [role] (role2) (role3)...`** | Sets an autorole, or several if serveral are specified. |
| **`autorole now`** | Displays the list of current autoroles on the server. |
| **`autorole reset`** | Disables autoroles on the server. |

### Enable the OwO mod

{% hint style="info" %}
This command converts Watora's answers to OwO language.
{% endhint %}

To enable Watora's OwO mod you have to use `owo`

| Usage | Help |
| :--- | :--- |
| **`owo (text)`** | Enables or disables the Watora's OwO mod. Otherwise if a text is specified, returns an owofied text. |

## Music Server Settings

### Set a DJ Role

{% hint style="danger" %}
DJs have more music permissions than regular users.  
Member with a DJ role can uses every musical commands.
{% endhint %}

{% hint style="info" %}
A role called DJ grants DJ permissions.
{% endhint %}

To set a DJ role you have to use `setdj` to learn more things about DJ permissions, take a look to this.

| Usage | Help |
| :--- | :--- |
| **`setdj [role] (role2) (role3)...`** | Configures a role as a DJ role \(or several\). |
| **`setdj reset`** | Removes the DJ permissions of every role on the server. |
| **`setdj now`** | Displays every roles with the DJ permissions. |
| **`setdj everyone`** | Grants Watora's DJ permissions to everyone on the server. |

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

### How to use music commands with reactions

{% hint style="info" %}
Only `skip, volume, pause, repeat, replay, previousnow, shuffle, stop` are available with reactions.
{% endhint %}

To use music commands with reaction you have to enable the lazy mod by using `lazy`

| Usage | Help |
| :--- | :--- |
| **`lazy`** | Enables or disables Watora's Lazy Mod. |



