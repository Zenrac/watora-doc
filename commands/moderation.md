---
description: Help with moderation commands.
---

# Moderation

{% hint style="info" %}

**Reminder :**

`command (optional) [required] [choice|choice_2]`

* Parameters between parenthesis are optional.
* Parameters between square brackets are required.
* Parameters separated by vertical bars means that you have to choose one of them. 
* Any characters outside parenthesis and brackets are supposed to be written.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>kick [user]</code></b>
      </td>
      <td style="text-align:left">Kicks a user from the server.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>ban [user]</code></b>
      </td>
      <td style="text-align:left">Kicks a user from the server.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>hackban [ID]</code></b>
      </td>
      <td style="text-align:left">Bans a user from the server with his ID.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>voicekick [user]</code></b>
      </td>
      <td style="text-align:left">Kicks a user from a voice channel.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>clean (num_msg)</code></b>
      </td>
      <td style="text-align:left">
        <p>Cleans up (num_msg) of Watora commands from the channel.</p>
        <p><em>num_msg is 100 if not specified.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>purge (num_msg)</code></b>
      </td>
      <td style="text-align:left">
        <p>Removes up to (num_msg) messages posted in chat.</p>
        <p><em>num_msg is 100 if not specified.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>stfu (num_msg)</code></b>
      </td>
      <td style="text-align:left">
        <p>Removes up to (num_msg) messages posted in chat from a user.</p>
        <p><em>num_msg is 100 if not specified.</em>
        </p>
      </td>
    </tr>
  </tbody>
</table>