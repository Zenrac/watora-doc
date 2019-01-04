---
description: Everything you must know about Autoplaylists.
---

# Autoplaylists

## Introduction

Autoplaylists are one of the most important feature of Watora, it allows to autoplay songs forever while the autoplaylist is enabled. You can create as much autoplaylists as you want, and you can use them everywhere, whatever if you created it on another server.

## Manage autoplaylists

To manage autoplaylists you have to use `pl`

| Usage | Help |
| :--- | :--- |


| **`pl (start) (autoplaylist)`** | Starts an autoplaylists. _If you don't specify an autoplaylist it loads your_ [_personal autoplaylists._](autoplaylists.md#personal-autoplaylist) |
| :--- | :--- |


| **`pl new [autoplaylist]`** | Creates a new autoplaylist with the specified name. |
| :--- | :--- |


| **`pl add (keywords|URL)`** | Adds a song to the current autoplaylist. _If you don't specify an URL nor keywords, adds the current song to the autoplaylist._ |
| :--- | :--- |


| **`pl remove (keywords|URL)`** | Removes a song to the current autoplaylist. _If you don't specify an URL nor keywords, removes the current song from the autoplaylist._ |
| :--- | :--- |


| **`pl now`** | Displays the current autoplaylist. |
| :--- | :--- |


| **`pl off`** | Disables the current autoplaylist. |
| :--- | :--- |


| **`pl repair (autoplaylist)`** | Repairs an autoplaylist. _If you don't specify one, repairs the current autoplaylist._ |
| :--- | :--- |


| **`pl info (autoplaylist)`** | Gives information about an autoplaylist. _If you don't specify one, about the current autoplaylist._ |
| :--- | :--- |


| **`pl clear (autoplaylist)`** | Deletes an autoplaylist and all of its content. _Warning : This operation cannot be undone._ |
| :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b><code>pl clone (autoplaylist)</code></b>
      </th>
      <th style="text-align:left">
        <p>Creates an autoplaylist by copying an existing autoplaylist.</p>
        <p><em>If you don't specify one, clones the current autoplaylist.</em>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table><table>
  <thead>
    <tr>
      <th style="text-align:left"><b><code>pl settings (autoplaylist)<br />(--edit [private|shuffle<br />|whitelist])</code></b>
      </th>
      <th style="text-align:left">
        <p>Displays information about an autoplaylist or edits its settings.</p>
        <p><em>See</em>  <a href="autoplaylists.md#autoplaylist-permissions"><em>Autoplaylist permissions</em></a>  <em>for more information.</em>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
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

| Usage | Help |
| :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b><code>pl set (autoplaylist) --edit private (True|False)</code></b>
      </th>
      <th style="text-align:left">
        <p>Manages if the autoplaylist is private or not.</p>
        <p><em>If no value is specified, invert the current value.</em>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table><table>
  <thead>
    <tr>
      <th style="text-align:left"><b><code>pl set (autoplaylist) --edit shuffle (True|False)</code></b>
      </th>
      <th style="text-align:left">
        <p>Manages if the autoplaylist is auto shuffled when playing or not.</p>
        <p><em>If no value is specified, invert the current value.</em>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>| **`pl set (autoplaylist) --edit whitelist (+|-) [user]`** | Edits the Whitelist to chose who can edit the autoplaylist. |
| :--- | :--- |


{% hint style="info" %}
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
Only whitelist people you trust. Or clone your autoplaylist somewhere to have a backup.
{% endhint %}

{% hint style="info" %}
You can start your personal autoplaylist by writing `pl`
{% endhint %}

{% hint style="info" %}
You can create shortener to start an autoplaylist \(and maybe avoid to mention someone each time you want to start his personal autoplaylist\). Take a look to [Custom Commands](https://github.com/Zenrac/watora-doc/tree/7b033c075b35be8a31e48251c038c193f9441d95/features/custom-commands-1.md).
{% endhint %}

### Autoplaylist settings

{% hint style="info" %}
Use `pl set (autoplaylist)` to display current autoplaylist settings.
{% endhint %}

#### Shuffle :

_Enabled by default._

Defines if songs are randomly played, or if the autoplaylist should be read in order.

