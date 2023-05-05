# Instructions for installing Minecraft forge on Linux: 
> note the following tutorial is only for version 1.18.2 

To install via the command line there is a few packages you need first.
Run this commands in your terminal:
`sudo apt-get -y unzip wget`

In your command line paste the following lines: 
```
  mkdir minecraftforge && \
  cd minecraftforge && \
  wget "https://maven.minecraftforge.net/net/minecraftforge/forge/1.18.2-40.2.0/forge-1.18.2-40.2.0-mdk.zip" -O temp.zip && \
  unzip temp.zip && \
  rm temp.zip
  
```
the above code makes a folder called minecraftforge, then it moves you into that folder and pulls minecraft 1.18.2 from the minecraft forge website and stores it into a temporary zip file, unzip is then used to unzip the folder into the current folder (minecraftforge) and then `rm` removes the zip folder

## Then install JDK 17 
- `sudo apt update` : updates the packages before installing java
- `sudo apt install openjdk-17-jdk` : Installs Java 17

## Install IntelliJ
```
wget "https://download-cdn.jetbrains.com/idea/ideaIC-2021.2.3.tar.gz" && tar xvf ideaIC-2021.2.3.tar.gz && mv idea-IC-212.5457.46/ /opt/idea && rm ideaIC-2021.2.3.tar.gz
```
the process above is the same as the minecraft install but instead of installing in the minecraftforge folder it is downloading and using tar to unpack and install, `mv` is then used to move the software into `/opt/idea` and then `rm` removes the tar.gz 



#### To play
From the minecraftforge directory run the command:
`./gradlew runClient`



Awesome, you now should be able play minecraft! 

