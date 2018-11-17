---
description: Everything you want to know about Watora's Permissions
---

# Permissions

{% hint style="info" %}
Watora public invitations don't generate an useless role when joining your server. 
{% endhint %}

{% hint style="info" %}
You can use`settings`to display current Watora's settings.
{% endhint %}

## Watora's Permissions Logic

Watora's permissions are mostly based on your channel/guild permissions.

#### Exemples :

* You cannot use the ban command if you cannot ban users.
* You cannot use the purge command if you cannot manage messages.

{% hint style="info" %}
To manage Watora's setting you need at least the `manage guild`permission.
{% endhint %}

## Music Permissions

Watora's music permissions are based on a DJ role system.

#### You are a DJ when you can verify one of the following line :

* You have a [DJ role](settings.md#set-a-dj-role)
* You have at least the manage guild permission
* You are alone in the voice channel with Watora

#### DJ permissions :

* It allows to use every musical commands without necessarily having high permissions on the server.
* It allows to use musical commands without being in the voice channel.

## How to limit Watora's commands

{% hint style="danger" %}
Users with at least the`manage guild`permissions aren't affected by this limitations.
{% endhint %}

### How to disable Watora on one or several channels

* You can use `ignore` to ignore one channel.
* You can use `bind` to disable Watora on every channels excepted one.

| Usage | Help |
| :--- | :--- |
| **`ignore (channel)`** | Disables Watora's commands on a channel.  _Current channel if not specified._ |
| **`bind (channel)`** | Binds Watora's commands to a channel.  _Current channel if not specified._ |

### How to disable Watora to several users or roles

You have to use `blacklist` to blacklist users or roles

| Usage | Help |
| :--- | :--- |
| **`blacklist add [user|role]`** | Adds a user to the guild blacklist. |
| **`blacklist remove [user|role]`** | Removes a user or a role from the guild blacklist. |
| **`blacklist clear`** | Clears the guild blacklist. |
| **`blacklist list`** | Displays the guild blacklist content. |

### How to disable a Watora's command

{% hint style="info" %}
You can't disable a customcommand. Instead, delete it.
{% endhint %}

To disable a command you have to use `disabledcommand` \(also called`dc)`

| Usage | Help |
| :--- | :--- |
| **`dc add [command]`** | Disables a command and his aliases on the server. |
| **`dc delete [command]`** | Enables anew a disabled command. |
| **`dc list`** | Displays the disabled commands list. |

