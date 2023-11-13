# Workshop Plugin Minecraft

In this workshop you will learn how to create a plugin minecraft for your server.

## Prerequisites :
You can work on Linux or Windows as you want.

- [Java Development Kit 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Visual Studio Code](https://code.visualstudio.com/download)
- And the game Minecraft 1.20

## Docs
[Spigot Doc](https://hub.spigotmc.org/javadocs/spigot/index.html)

## Step 0
Clone the repository and open on your favorite IDE. Then open a terminal in the repository and run this command :

```mvn install```

## Step 1 - Create plugin.yml
For your plugin to launch, you need to fill in the **plugin.yml** file in the resources folder.

[Create a plugin.yml](https://www.spigotmc.org/wiki/plugin-yml/#required-attributes)

## Step 2 - Start the plugin
To start your plugin you need to complete the main file App.java

Add **onEnable** and **onDisable** methods and print something in console for this two methods.

When the plugin is starting it must display : ``Plugin is load !``

When the plugin is starting it must display : ``Plugin is unload !``

[Spigot Doc](https://hub.spigotmc.org/javadocs/spigot/index.html)

## Step 3 - Compile and test

To compile your plugin you need to re-run this command : 

```mvn install```

After that you need to start your server, go to the server folder, and run the script corresponding to your OS :

```Linux/Mac : start.sh```

```Windows : start.bat```

When your server is start you can put your plugins in to the plugins folder of the server. The plugin file is located in the repository root after compilation.

And then run the command : ``reload`` in the console of your server and your plugin will be load and you can see your message in the console.

## Step 4 - Join Message

Now you need to change the message when a player joins the server.

The expected result is :

``{playerName} has joined ! ({currentPlayerOnline} / {maxSlotsServer})``

Bonus : Add some colors in your message :)

[Events API](https://www.spigotmc.org/wiki/using-the-event-api/)

## Step 5 - Create custom Commands

After that create 2 commands : 

``/hello`` That send a message to the player who executed the command
``/broadcast <msg>`` That send the message to all the server

[Commands](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/command/Command.html)

## Step 6 - Create custom Items

Let's try to create some custom items.

First give a **Compass** to the player in his first slot of his inventory bar when he join the server.

Then create a **Nether Star** with a name, and a little description.

Finally create a **Sword** with Sharpness 10 and the name Excalibur

[ItemStack](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/inventory/ItemStack.html)



