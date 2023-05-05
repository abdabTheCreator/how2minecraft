# Instructions for installing Minecraft forge on Linux: 
> note the following tutorial is only for version 1.18.2 

- Visit [Minecraft forge 1.18.2](https://files.minecraftforge.net/net/minecraftforge/forge/index_1.18.2.html)
- Choose download recomended > MDK 
Unzip the downloaded folder 
- `cd` into the unzipped folder 
- `./gradlew genEclipseRun` : This command builds the dependecies that are set out in the gradle.properties file and sets up the clients to be able to play minecraft

## Next install IntelliJ 
> IntelliJ is a IDE that will be used to program the mods using Java 
- Run the following command in your terminal: `sudo snap install intellij-idea-ultimate --classic`

## Then install JDK 17 
- `sudo apt update` : updates the packages before installing java
- `sudo apt install openjdk-17-jdk` : Installs Java 17

#### To play
`./gradlew runClient`



Awesome, you now should be able play minecraft! 

