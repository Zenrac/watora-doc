---
description: Everything you need to know about Autoplaylists.
---

# Autoplaylists

## Introduction

Autoplaylists are one of the most important features of Watora, it allows you to autoplay songs forever while the autoplaylist is enabled. You can create as many autoplaylists as you want, and you can use them everywhere, even if you created them on another server.

## Manage autoplaylists

To manage autoplaylists you have to use `pl`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>pl (start) (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Starts an autoplaylist.
        <br /><em>If you don&apos;t specify an autoplaylist it loads your </em><a href="autoplaylists.md#personal-autoplaylist"><em>personal autoplaylist.</em></a>&lt;em&gt;&lt;/em&gt;</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl new [autoplaylist]</code></b>
      </td>
      <td style="text-align:left">Creates a new autoplaylist with the specified name.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl add (keywords|URL|current_queue)</code></b>
      </td>
      <td style="text-align:left">
        <p>Adds a song to the current autoplaylist.
          <br /><em>If you don&apos;t specify an URL or keywords, this will add the current song to the autoplaylist.</em>
        </p>
        <p><em>You can write current_queue to add the whole current queue to the autoplaylist.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl remove (keywords|URL)</code></b>
      </td>
      <td style="text-align:left">Removes a song from the current autoplaylist.
        <br /><em>If you don&apos;t specify an URL or keywords, this will remove the current song from the autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl now</code></b>
      </td>
      <td style="text-align:left">Displays the current autoplaylist.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl off</code></b>
      </td>
      <td style="text-align:left">Disables the current autoplaylist.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl repair (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Repairs an autoplaylist.
        <br /><em>If you don&apos;t specify one, this will repair the current autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl info (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Gives information about an autoplaylist.
        <br /><em>If you don&apos;t specify one, this will target the current autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl clear (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Deletes an autoplaylist and all of its content.
        <br /><em>Warning: This operation cannot be undone.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl clone (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">
        <p>Creates an autoplaylist by copying an existing autoplaylist.</p>
        <p><em>If you don&apos;t specify one, this will clone the current autoplaylist.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl settings (autoplaylist) <br />(--edit [private|shuffle<br />|whitelist|description| avatar])</code></b>
      </td>
      <td style="text-align:left">
        <p>Displays information about an autoplaylist or edits its settings.</p>
        <p><em>See </em><a href="autoplaylists.md#autoplaylist-permissions"><em>Autoplaylist permissions </em></a><em>for more information.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl find (query)</code></b>
      </td>
      <td style="text-align:left">Searches for an autoplaylist sorted by upvote.
        <br />You can specify a query to narrow your search.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl upvote (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">
        <p>Upvotes an autoplaylist.</p>
        <p>Autoplaylists with more upvotes have more visibility.</p>
      </td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
You can use `pl`instead of `pl start`
{% endhint %}

#### Things to know :

* You can create as many autoplaylists as you want, but only one personal autoplaylist.
* Your autoplaylist can have as many songs as you want.

## Types of Autoplaylists

Basically there are two types of Autoplaylists. 

### Basic Autoplaylist

#### An autoplaylist has :

* A name \(chosen when created\)
* Songs \(added or removed with `pl add` and `pl remove)`
* Settings
* Permissions

### Personal Autoplaylist

Personal and Basic autoplaylists share the same attributes except that the Personal autoplaylist doesn't have a name.  
It's called **your autoplaylist**.

It also means that when calling a Personal Autoplaylist the argument passed will change. Instead of using `(autoplaylist)`, use `(user_mention)` instead.

**Examples :**

![Using only pl instead of pl start and mentioning someone loads their personal autoplaylist](../.gitbook/assets/image%20%283%29.png)

![Mentioning myself to display my personal autoplaylist settings](../.gitbook/assets/image%20%287%29.png)

## Autoplaylist Configuration

### Editing Autoplaylists

<table>
  <thead>
    <tr>
      <th style="text-align:left">Usage</th>
      <th style="text-align:left">Help</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>pl set (autoplaylist) --edit private (True|False)</code></b>
      </td>
      <td style="text-align:left">
        <p>Manages the autoplaylist  privacy settings.</p>
        <p><em>If no value is specified, this will act as a toggle.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl set (autoplaylist) --edit shuffle (True|False)</code></b>
      </td>
      <td style="text-align:left">
        <p>Manages the autoplaylist auto-shuffle setting.</p>
        <p><em> If no value is specified, this will act as a toggle.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl set (autoplaylist) --edit whitelist (+|-) [user]</code></b>
      </td>
      <td style="text-align:left">Edits the Whitelist and allows you to chose who can edit the autoplaylist.</td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
You can use`pl set`as an alias for `pl settings`
{% endhint %}

### Autoplaylist permissions

* By default, an autoplaylist is Private and the Whitelist is empty.
* Anyone can start any autoplaylist.
* You cannot edit a private Autoplaylist if you're not in the Whitelist.
* You can edit a public Autoplaylist.

#### Private Autoplaylist

| Permission | Everyone | Whitelisted User | Creator |
| :--- | :--- | :--- | :--- |
| Start autoplaylist | **Yes** | **Yes** | **Yes** |
| Clone autoplaylist | **Yes** | **Yes** | **Yes** |
| Add a song to the autoplaylist | No | **Yes** | **Yes** |
| Remove a song from the autoplaylist | No | **Yes** | **Yes** |
| Repair the autoplaylist | No | **Yes** | **Yes** |
| Clear the playlist | No | No | **Yes** |

#### Public Autoplaylist

| Permission | Everyone | Whitelisted User | Creator |
| :--- | :--- | :--- | :--- |
| Start autoplaylist | **Yes** | **Yes** | **Yes** |
| Clone autoplaylist | **Yes** | **Yes** | **Yes** |
| Add a song to the autoplaylist | **Yes** | **Yes** | **Yes** |
| Remove a song from the autoplaylist | **Yes** | **Yes** | **Yes** |
| Repair the autoplaylist | **Yes** | **Yes** | **Yes** |
| Clear the playlist | **Yes** | **Yes** | **Yes** |

{% hint style="danger" %}
In almost every case you should set your autoplaylist to Private.
{% endhint %}

{% hint style="warning" %}
Either only whitelist people you trust or clone your autoplaylist somewhere as a backup.
{% endhint %}

{% hint style="info" %}
You can start your personal autoplaylist by using `pl`
{% endhint %}

{% hint style="info" %}
You can create an alias to start an autoplaylist \(and avoid  mentioning someone each time you want to start their personal autoplaylist\). Take a look at [Custom Commands](custom-commands.md).
{% endhint %}

### Autoplaylist settings

{% hint style="info" %}
Use `pl set (autoplaylist)` to display the current autoplaylist settings.
{% endhint %}

#### Shuffle :

_Enabled by default._

Defines if the songs are randomly played, or played in order.

### Telling the autoplaylist to start a song at a specified timecode

You can do this by adding **`?t=SECONDS`** __at the end of your url when adding the song \(it also works with the play command\).

{% hint style="info" %}
**Examples:**   
**pl add** [**https://youtu.be/UQpRzyNXDBg?t=120**](https://youtu.be/UQpRzyNXDBg?t=120) **``**  
**pl add** [**https://soundcloud.com/user-345751583/opening-recreator-full-gravity-wall?t=60**](https://soundcloud.com/user-345751583/opening-recreator-full-gravity-wall?t=60)\*\*\*\*
{% endhint %}



