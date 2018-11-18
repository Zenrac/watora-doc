---
description: Everything you must know about Autoplaylists.
---

# Autoplaylists

## Introduction

Autoplaylists are one of the most important feature of Watora, it allows to autoplay songs forever while the autoplaylist is enabled. You can create as much autoplaylists as you want, and you can use them everywhere, whatever if you created it on another server.

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
      <td style="text-align:left">Starts an autoplaylists.
        <br /><em>If you don't specify an autoplaylist it loads your </em><a href="autoplaylists.md#personal-autoplaylist"><em>personal autoplaylists.</em></a><em></em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl new [autoplaylist]</code></b>
      </td>
      <td style="text-align:left">Creates a new autoplaylist with the specified name.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl add (keywords|URL)</code></b>
      </td>
      <td style="text-align:left">Adds a song to the current autoplaylist.
        <br /><em>If you don't specify an URL nor keywords, adds the current song to the autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl remove (keywords|URL)</code></b>
      </td>
      <td style="text-align:left">Removes a song to the current autoplaylist.
        <br /><em>If you don't specify an URL nor keywords, removes the current song from the autoplaylist.</em>
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
        <br /><em>If you don't specify one, repairs the current autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl info (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Gives information about an autoplaylist.
        <br /><em>If you don't specify one, about the current autoplaylist.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl clear (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">Deletes an autoplaylist and all of its content.
        <br /><em>Warning : This operation cannot be undone.</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl clone (autoplaylist)</code></b>
      </td>
      <td style="text-align:left">
        <p>Creates an autoplaylist by copying an existing autoplaylist.</p>
        <p><em>If you don't specify one, clones the current autoplaylist.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl settings (autoplaylist) <br />(--edit [private|shuffle<br />|whitelist])</code></b>
      </td>
      <td style="text-align:left">
        <p>Displays information about an autoplaylist or edits its settings.</p>
        <p><em>See </em><a href="autoplaylists.md#autoplaylist-permissions"><em>Autoplaylist permissions </em></a><em>for more information.</em>
        </p>
      </td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
You can use `pl`instead of `pl start`
{% endhint %}

#### Things to know :

* You can create as much autoplaylists as you want. But only one personal autoplaylist.
* Your autoplaylist can have as much song as you want.

## Types of Autoplaylist

Basically there are two types of Autoplaylists. 

### Basic Autoplaylist

#### An autoplaylist has :

* A name \(choosen when created\)
* Songs \(added or removed with `pl add` and `pl remove)`
* Settings
* Permissions

### Personal Autoplaylist

A Personal autoplaylist share the same attributes except that it doesn't have a name.  
It's called **your autoplaylist**.

It also means that `(autoplaylist)` in commands becomes `(user_mention)`.

**Examples :**

![Using only pl instead of pl start and mentionning someone to load his personal autoplaylist](../.gitbook/assets/image%20%283%29.png)

![Mentionning myself to display my personal autoplaylist settings](../.gitbook/assets/image%20%286%29.png)

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
        <p>Manages if the autoplaylist is private or not.</p>
        <p><em>If no value is specified, invert the current value.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl set (autoplaylist) --edit shuffle (True|False)</code></b>
      </td>
      <td style="text-align:left">
        <p>Manages if the autoplaylist is auto shuffled when playing or not.</p>
        <p><em>If no value is specified, invert the current value.</em>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b><code>pl set (autoplaylist) --edit whitelist (+|-) [user]</code></b>
      </td>
      <td style="text-align:left">Edits the Whitelist to chose who can edit the autoplaylist.</td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
You can use`pl set`as an alias for `pl settings`
{% endhint %}

### Autoplaylist permissions

* By default, an autoplaylist is Private and the Whitelist is empty.
* Everyone can start every autoplaylist.
* You cannot edit a private Autoplaylist if you're not in the Whitelist.
* You can edit a public Autoplaylist.

#### Private Autoplaylist

| Permission | Everyone | Whitelisted User | Creator |
| :--- | :--- | :--- | :--- |
| Start the autoplaylist | **Yes** | **Yes** | **Yes** |
| Clone the autoplaylist | **Yes** | **Yes** | **Yes** |
| Add a song in the autoplaylist | No | **Yes** | **Yes** |
| Remove a song from the autoplaylist | No | **Yes** | **Yes** |
| Repair the autoplaylist | No | **Yes** | **Yes** |
| Clear the playlist | No | No | **Yes** |

#### Public Autoplaylist

| Permission | Everyone | Whitelisted User | Creator |
| :--- | :--- | :--- | :--- |
| Start the autoplaylist | **Yes** | **Yes** | **Yes** |
| Clone the autoplaylist | **Yes** | **Yes** | **Yes** |
| Add a song in the autoplaylist | **Yes** | **Yes** | **Yes** |
| Remove a song from the autoplaylist | **Yes** | **Yes** | **Yes** |
| Repair the autoplaylist | **Yes** | **Yes** | **Yes** |
| Clear the playlist | **Yes** | **Yes** | **Yes** |

{% hint style="danger" %}
In almost every case you should let your autoplaylist Private.
{% endhint %}

{% hint style="warning" %}
Only whitelist people you trust in, or clone your autoplaylist somewhere to have a backup.
{% endhint %}

{% hint style="info" %}
You can start your personal autoplaylist by writing `pl`
{% endhint %}

{% hint style="info" %}
You can create shortener to start an autoplaylist \(and maybe avoid to mentionning someone each time you want to start his personal autoplaylist\). Take a look to [Custom Commands](custom-commands-1.md).
{% endhint %}

### Autoplaylist settings

{% hint style="info" %}
Use `pl set (autoplaylist)` to display current autoplaylist settings.
{% endhint %}

#### Shuffle :

_Enabled by default._

Defines if songs are randomly played, or if the autoplaylist should be read in order.

