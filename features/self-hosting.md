---
description: >-
  In order to avoid YouTube ratelimits and to get more features (such as playing
  local files), you can self host Watora's music.
---

# Self hosting

## Requirements

Download ****[Watora\_Server.zip](https://drive.google.com/open?id=10F0Bpy4xaptOMn-hTP6QOEf96OrXguKI)  
****Java 11+ \(you can download [Java 13 here](https://www.oracle.com/java/technologies/javase-jdk13-downloads.html)\)

## Get Started

### **Extract `Watora_Server.rar` somewhere, and open the extracted folder**

**This folder should contain 3 files.**

### **Edit `application.yml` with a text editor**

Set an opened port at line 2  
****Set a password at line 5

### **Start `launcher.bat`**

A terminal showing "Lavalink" should open. If a firewall pop up ask for permission, grants permission to Java to access public network.

### **Use Watora `hostconfig` command in DMs to allow her to connect**

She'll need to know your IP, your port and the password you have chosen in order to create a connection.

## **Bonus**

If you want to play local files, you can set local at line 17 to true in `application.yml`  
****Issuing `=play full/path/to/your/file.mp3` will allow Watora to play your file

