# Custom Commands

{% hint style="warning" %}
Custom Commands are [Rich Commands](rich-commands.md).  
It's highly recommended to read the [Rich Commands page](rich-commands.md) before reading this page.
{% endhint %}

## Custom Commands Basics

### Manage Custom Commands

To manage custom commands on your server you have to use `customcommand` \(or `cc`\)

| Usage | Help |
| :--- | :--- |
| **`cc add [command] [content]`** | Allows to add a custom command on the server.  |
| **`cc edit [command] [content]`** | Allows to edit a custom command on the server.  |
| **`cc delete [command]`** | Allows to remove a custom command from the server.  |
| **`cc list`** | Displays the custom commands list. |
| **`cc raw [command]`** | Displays the real content of a custom command. |

**Example :**

![Simple custom command](../.gitbook/assets/image%20%281%29.png)

### Creating a allias

To create an alias you can use the fact that [you can call a command](rich-commands.md#you-can-call-a-command) with Rich Commands.

![The letter k is now an allias for roll](../.gitbook/assets/image%20%282%29.png)

{% hint style="info" %}
When creating the custom command, you can specify a static parameter for the command, for example`>>>roll 10`will call `roll 10`when using`k` 
{% endhint %}

### Commands which doesn't need any parameter

Here's an example of a russian roulette which either play an earrape, or a relaxing song.

![Haha, I got lucky](../.gitbook/assets/image%20%2812%29.png)

### Mixing two commands together

You can call several commands thanks to`&&`

**Example :**

![Same example than Rich Command one, but in a custom command.](../.gitbook/assets/image%20%289%29.png)

* Every variables mentionned in [Rich Commands](rich-commands.md)

## Custom Commands Advanced

### How to get user's parameter

If you don't want a static parameter, you can ask the user to give one.

| Number | Effect |
| :--- | :--- |
| **`x`** | Empty. |
| **`&`** | Same than`0`but without counting quotations |
| **`0`** | Gives every words. |
| **`1`** | Gives the first word. |
| **`2`** | Gives the second word. |
| **`3`** | Gives the third word. |
| ... | ... |

{% hint style="info" %}
Using quotations between a group of words allows to get several words instead of taking one by one word.  
  
**Example :**   
`cmd "This is a test" Hello "Help please"`  
{1} = This is a test  
{2} = Hello  
{3} = Help please
{% endhint %}

**Example :**

![](../.gitbook/assets/image%20%288%29.png)

{% hint style="info" %}
By default, if you only specify `>>>volume`without`{1}`it's the same thing than `>>>volume {0}` it means that every parameters are taken, when`{1}`only takes the first one.
{% endhint %}

### Conditions

You can set a default value when failing to catch a value.

**Example :**

![When calling =vm, I didn&apos;t specify a third parameter, it returns Cool Song](../.gitbook/assets/image.png)

### Others

#### You can select several parameters based on their index. 

**Example :**

```text
cmd This is an example

{1:3} = This is an
{-1} = example
{-1:-2} = example an
```

{% hint style="info" %}
You can use negative number to start counting from the end
{% endhint %}

