---
description: >-
  In order to avoid YouTube ratelimits and to get more features (such as playing
  local files), you can self host Watora's music.
---

# Self Hosting

{% hint style="info" %}
Self Hosting requires a server \(download and installation below\) which is also called a **node**.   
To make her use yours, you'll have to connect your node to Watora by using **`hostconfig`**.
{% endhint %}

## Requirements

Download ****[Watora\_Server.zip](https://drive.google.com/open?id=10F0Bpy4xaptOMn-hTP6QOEf96OrXguKI)  
****Java 11+ \(you can download [Java 13 here](https://www.oracle.com/java/technologies/javase-jdk13-downloads.html)\)

## Get Started

### **Extract `Watora_Server.rar` somewhere, and open the extracted folder**

This folder should contain 3 files.  
  
**Lavalink.jar** : The Java server.   
**application.yml** : The configuration file which allows to edit the configuration of the node.  
**run.bat** : A script for Windows user to start your node quickly by launching it.

### **Edit `application.yml` with a text editor**

* Set an **opened port** at **line 2**.  Default port is 2333. For instance, if you already opened a port for a Minecraft server \(port 25565\), and you're not using it anymore, you can use it here.  Otherwise, you'll have to open a port and make it redirect to your computer. You can follow any tutorial on the Internet, like [this one](https://alienbunker.com/2017/open-ports-minecraft-server-2017-version/) based on Minecraft Ports. 
* Set a **password** at **line 5**. Default password of Lavalink is youshallnotpass. This is roughly recommended to change it for something else.

### **Start your node**

On Windows, launch it with**`launcher.bat`**  
On Linux , use**`java -jar Lavalink.jar`**  
  
A terminal showing "Lavalink" should open.  
If a firewall pop-up asks for permission, accept to grant permission to Java to access public network.

### **Use Watora `hostconfig` command in DMs to allow her to connect**

She'll need to know your IP, your port and the password you have chosen in order to create a connection.

## **Bonus**

If you want to play local files, you can set local at line 17 to true in `application.yml`  
****Issuing `=play full/path/to/your/file.mp3` will allow Watora to play your file.

