# Minecraft Cloud Shell (or anywhere cloud services) Tutorial & Info

In this project, we'll teach you host your very own Java/Bedrock Minecraft Server using `Google Cloud Shell`. This works under `Ubuntu/Debian` based Linux operation system. This project requires **NO CREDIT CARD** and the whole project is entirely **FREE**! You can make a server without costing you anything.

**The following features are added into this project are:**

- Supports many type of Java Servers (Base on https://mcutils.com API)
- Clean & Friendly Interface
- Support with Vanilla Bedrock Server
- Added Server Management
- Easy to use (Easier functional scripts)
- Instant EULA script setup _(Completely skipping this part whice makes it easier)_
- Instant and Faster Server Installation _(It would probably take you like approx 40 seconds to setup a server)_

## Need help?

> [**Submit any Issues here**](https://github.com/hapis1703/minecraftserver/issues)

### Server Specs:

- **OS:** Debian GNU/Linux 10 (buster) x86_64
- **RAM:** 8GB to 16GB
- **Location:** Based on your physical location.
- **Storage:** Approx 5GB
- **CPU:** AMD EPYC (2) 7B12 @ 2.249GHz or Intel Xeon (4) @ 2.199GHz

### Service Used:

- [playit.gg](https://playit.gg)
- [SDKMAN](https://sdkman.io)
- [Google Cloud Shell](https://cloud.google.com/shell)

## Installation

- Activate a [Google Cloud Shell](https://cloud.google.com/shell)
- Run Installation Script:

```
bash <(curl -s https://raw.githubusercontent.com/hapis1703/minecraftserver/main/install)
```

Follow the installation step shown in the console

- Go to your server directory:

```
cd server
```

- Start your server:

```
./start
```

## Join your server

- To join your server, start your server by doing: `./start` _(If you haven't started it yet)_ and do this command:

```
screen -r playit
```

- Now click the **Claim URL** and it should show you your host IP and Tunnel Server.
- Once your in that page, scroll down and click **Add Tunnel** on Minecraft Java/Bedrock and next to the **Local server address**, click **Add**.
- Now copy the generated dedicated IP something along with `auto.playit.gg` and copy it into the Server Address in Minecraft and now you can play the server.

## Accessing Server Console

- To access the server console, run this command:

```
screen -r server
```

To completely stop the server, you can do `./stop` on the console or do `exit` or `stop` on the Minecraft console

## Detaching Screen/Session

- To detach the screen you can do it using the following keyboard shortcut
  `CTRL + A` then press `D`

## Cracked Launcher

- If you're using cracked version of **Minecraft Java Edition**

- Go to `server.properties` and find the properties `online-mode`:

```
nano server.properties
```

- Change it from `true` to `false`

```
online-mode=false
```

- Save and exit the file by pressing `CTRL + X` then press `Y` and press `Enter` exit the text editor.

- Restart your server

## Access Server Files

If you want to access your server files, go to `Open Editor` on the top right.

- Once you there, if you don't see any folders on the left side, you can `Open Folder` and pick `server` to view and modify anything inside.
- If you made any changes on your server, restart your server.
  After you restarted your server, all the changes are saved into your server.

## Supported Server Type:

Minecraft Java Edition:

- **Fabric**
- **Folia**
- **Forge**
- **Paper**
- **Pufferfish**
- **Purpur**
- **Vanilla**

Minecraft Bedrock Edition:

- **Vanilla**

_(We'll add more server type in this project soon!)_

## Restart the Server

If you don't know how to restart the server, here is the step.

- Go to `server` directory and do this command.
- Stop the server mean you stop both the Minecraft Server and Playit.gg:

```
./stop
```

- And now start your server again:

```
./start
```

Now your server has fully restarted.

## Keeping the server Alive

There's only **ONE** way to keep your server online longer than 20 minutes:

- You must Keep your browser open to keep your server online. This so the shell doesn't get terminated when it's unused or the browser is closed.

_(Don't worry, your device that is being used to host your server isn't affected from the intensity of your server.)_

If you have any method the would possibly keep the server alive 24/7, feel free to **Fork** this project and request a **Pull** to this project. Any help will be greatly appreciated.

## Limitation of this project

### Google Cloud Shell Quota

While I was editing this project, I notice that Google has added a quota for each Cloud Shell uses and you can only host your server for the max of `50` hours per `Week`.
Once you used all of the hours, you can't use it again until next week.

### No Dedicated IP

Sadly you can't use the host IP into your dedicated IP as it won't let you join that server, you can only join your server by the generated dedicated IP provided by **playit.gg**. If you know how to reverse proxy the tunnel system, you _can_ actually use the host IP to make a dedicated IP for your server but I highly doubt that would ever happen.

### Mixed Server Specs

Each Cloud Shell session will have different specs of your server based on your physical location so you won't always get the best performance of your server but good news being that it's always the range between `8GB` to `16GB` so you won't have to worry about lag when playing in the server with high processing in your server.

## Conclusion

Now you can host your very own Minecraft Server for both Java & Bedrock fast and easy and it won't cost you a single penny to make a fast and strong server. Best of all, IT'S FOREVER! Feel free to leave any requests you would like me to add into the project. If you have any issues, go to the [**Issues**](https://github.com/hapis1703/minecraftserver/issues) tab and submit a issue there.
