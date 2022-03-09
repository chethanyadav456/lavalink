## How to make lavalink server

# What are we doing today

In this tutorial we will be setting up lavalink server! 🎉

---

Let's get started.

Now, first thing first

### Setting up the enviroment
**To make a lavalink server, you will need a java 13 or greater, I recommend using Azul Zulu java 16 or 17.**

You can download & setup java by going to here:
- [Linux](https://www.azul.com/downloads/?os=linux&package=jdk) (Make sure to get `zulu16-jdk` or `zulu17-jdk`
    - [Ubuntu / Debian; APT Base](https://docs.azul.com/core/zulu-openjdk/install/debian)
    - [Rhel / CentOS / Oracle; RPM Base](https://docs.azul.com/core/zulu-openjdk/install/rpm-based-linux)
    - [Arch; I use arch btw.](https://aur.archlinux.org/packages/zulu-16-bin/)
- [MacOS](https://www.azul.com/downloads/?os=macos&package=jdk)
- [Windows](https://www.azul.com/downloads/?os=windows&package=jdk)

If you want to host lavalink on replit. you can just click this button
[![Run on Repl.it](https://repl.it/badge/github/DarrenOfficial/lavalink-replit)](https://repl.it/github/DarrenOfficial/lavalink-replit)

Once install you can verify it by doing `java -version`, the output should look something like this

```bash
openjdk version "16.0.2" 2021-07-20
OpenJDK Runtime Environment Zulu16.32+15-CA (build 16.0.2+7)
OpenJDK 64-Bit Server VM Zulu16.32+15-CA (build 16.0.2+7, mixed mode, sharing)
```

depending on your os, you may need to restart to for it to apply.


**Congratulations 🥳 you’ve got Java installed!**

---
### Setting up lavalink.jar
To get started, you need to download the `lavalink.jar` and `application.yml` It’s pretty simple!

There are 2 jars provided below, one is the original one from [freyacodes](https://github.com/freyacodes) and one custom one made by [melike2d](https://github.com/melike2d) which has alot more features than the original one

#### Lavalink Jar download

- [Original Jar](https://github.com/freyacodes/Lavalink/releases/tag/3.4)
> https://github.com/freyacodes/Lavalink/releases/tag/3.4

    - [Dev Jar](https://github.com/freyacodes/Lavalink/tree/dev)
> https://ci.fredboat.com/repository/download/Lavalink_Build/.lastSuccessful/Lavalink.jar?guest=1&branch=refs/heads/dev

- [Custom Jar](https://github.com/melike2d/lavalink) 
> https://cdn.darrennathanael.com/jars/Lavalink.jar


#### application.yml download

- [Original Jar application.yml](https://github.com/freyacodes/Lavalink/blob/master/LavalinkServer/application.yml.example)

- [Custom Jar application.yml](https://cdn.darrennathanael.com/jars/application.yml)

> *Both are different*

Once you’ve downloaded the jar and application.yml file, you can simply edit the application.yml port and password to your preferences.

Now last step is to move both into a single folder, then open a terminal to that folder using `cd`
> [How to use cd in windows](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/)

> [How to use cd in mac](https://www.macworld.com/article/221277/command-line-navigating-files-folders-mac-terminal.html)

> If your on linux go figure out yourself nerd.

Then run it by doing `java -jar Lavalink.jar` or if you wanna limit it to only using X amount of ram you can do `java -XmxXG -jar Lavalink.jar` I.e. `java -Xmx2G -jar Lavalink.jar`


and you should get an output similar to this:
```bash
[root@darren-aws-testsrv lavalink]# java -Xmx2G -jar Lavalink.jar 
2021-12-03 04:22:25.402  INFO 1826146 --- [           main] lavalink.server.Launcher                 : 

       .   _                  _ _       _    __ _ _
      /\\ | | __ ___   ____ _| (_)_ __ | | __\ \ \ \
     ( ( )| |/ _` \ \ / / _` | | | '_ \| |/ / \ \ \ \
      \\/ | | (_| |\ V / (_| | | | | | |   <   ) ) ) )
       '  |_|\__,_| \_/ \__,_|_|_|_| |_|_|\_\ / / / /
    =========================================/_/_/_/

        Version:        3.3.2.3
        Build:          1239
        Build time:     31.08.2021 17:26:20 UTC
        Branch          main
        Commit:         2ad6b46
        Commit time:    31.08.2021 17:17:13 UTC
        JVM:            17.0.1
        Lavaplayer      1.3.93-original
```

---
## And that’s it! You’ve installed lavalink! 🎉🥳

Thank you for reading, have a great day!
