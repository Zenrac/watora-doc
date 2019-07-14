---
description: Everything you must know about how to create and use Custom Commands.
---

# Custom Commands

{% hint style="warning" %}
Custom Commands are [Rich Commands](rich-commands.md).  
It's highly recommended to read the [Rich Commands page](rich-commands.md) before reading this page.
{% endhint %}

## Custom Commands Basics

### Managing Custom Commands

To manage custom commands on your server you have to use `customcommand` \(or `cc`\)

| Usage | Help |
| :--- | :--- |
| **`cc add [command] [content]`** | Allows you to add a custom command on the server.  |
| **`cc edit [command] [content]`** | Allows you to edit a custom command on the server.  |
| **`cc delete [command]`** | Allows you to remove a custom command from the server.  |
| **`cc list`** | Displays the custom commands list. |
| **`cc raw [command]`** | Displays the real content of a custom command. |

**Example :**

![Simple custom command](../.gitbook/assets/image%20%281%29.png)

### Creating an alias

To create an alias you can use the fact that [you can call a command](rich-commands.md#you-can-call-a-command) with Rich Commands.

![The letter k is now an alias for roll](../.gitbook/assets/image%20%282%29.png)

{% hint style="info" %}
When creating the custom command, you can specify a static parameter for the command, for example`>>>roll 10`will call `roll 10`when using`k` 
{% endhint %}

### Commands which doesn't need any parameter

Here's an example of a russian roulette which either play an earrape, or a relaxing song.

![Haha, I got lucky](../.gitbook/assets/image%20%2813%29.png)

### Mixing several commands together

You can call several commands thanks to`&&`

**Example :**

![Same example than Rich Command one, but in a custom command.](../.gitbook/assets/image%20%2810%29.png)

## Custom Commands Advanced

### How to get user's parameter

If you don't want a static parameter, you can ask the user for one.

| Number | Effect |
| :--- | :--- |
| **`x`** | Empty. |
| **`&`** | Same as`0`but without counting quotations |
| **`0`** | Gives every words. |
| **`1`** | Gives the first word. |
| **`2`** | Gives the second word. |
| **`3`** | Gives the third word. |
| ... | ... |

{% hint style="info" %}
Using quotations between a group of words allows you to parse several words instead of parsing them one by one.  
  
**Example :**   
`cmd "This is a test" Hello "Help please"`  
{1} = This is a test  
{2} = Hello  
{3} = Help please
{% endhint %}

**Example :**

![](../.gitbook/assets/image%20%289%29.png)

{% hint style="info" %}
By default, if you only specify `>>>volume`without`{1}`it's the same thing as`>>>volume {0}` . This means that every parameter is parsed, when`{1}`used, the command will only take the first one.
{% endhint %}

### Conditions

You can set a default value to use when no arguments are passed.

**Example :**

![When calling =vm, since I didn&apos;t specify a third parameter, it returns Cool Song](../.gitbook/assets/image.png)

### Others

#### You can select several parameters based on their index. 

**Example :**

```text
cmd This is an example

{1:3} = This is an
{-1} = example
{-1:-2} = example an
{2:} = is an example
```

{% hint style="info" %}
You can use negative numbers to start counting from the end of the argument list.
{% endhint %}

