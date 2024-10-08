# microbot-launcher-linux

microbot-launcher-linux is a Linux Launcher for [Microbot](https://github.com/chsami/microbot)!

## How to use
NOTE: Requires Java 11 (Just like Microbot)

- Put the Launcher in the folder where you want to have the files organized.

- Launch using Terminal: ```java -jar microbot-launcher-linux.jar```

- Enjoy!

## Using a Jagex Account
You can use this with a Jagex Account, however you currently need to do some manual steps:

- Obtain a `credentials.properties` file from a RuneLite launcher. This can be from a Windows or Mac launcher aswell, see [here](https://github.com/runelite/runelite/wiki/Using-Jagex-Accounts).

You can however do this directly on Linux using the third-party [Bolt Launcher](https://github.com/Adamcake/Bolt/):

- Install Bolt Launcher from Flathub, see the link above for more info.

- After logging into Bolt Launcher, select RuneLite as the Game client.

- Go to the Application Options and click on Configure RuneLite

- In the window that pops up, paste the following argument for Client arguments: `--insecure-write-credentials` (Just like the guide from RuneLite above)

- Now if you start RuneLite, a `credentials.properties` file will be generated to the following path: `/home/YOUR-USERNAME/.var/app/com.adamcake.Bolt/data/bolt-launcher/.runelite/`

- Copy the `credentials.properties` file in to the `.runelite` folder at the following path (If you don't have a .runelite folder there, make sure to launch Microbot through the launcher once): `/home/YOUR-USERNAME/.runelite/`

- Now when you start Microbot through the Launcher again, it should work with your Jagex Account!

NOTE: There are probably other methods aswell. Feel free to share them!

## Features
- Automatically downloads the latest non-nightly .jar file from GitHub releases & puts it into a /microbot directory which gets created in the same folder as the launcher. Also deletes older versions and checks for newer ones.
- Launches the .jar file for you

## Contributions
Feel free to submit a pull request if you have any cool changes!
