# Explanation of PS2 Setup

## Metadata Start
The first piece of information the metadata needs is the Collection/Launch data

### Collection Information

```
Collection: Playstation 2
Shortname: PS2
Extensions: iso
Launch: /Applications/PCSX2-v1.7.2952.app {file.path} 
```
#### Console Info

##### Collection
Collection: `Playstation 2`  
This tells us what the collection should be called

##### Shortname
Shortname: `PS2`  
This is the short name for the console

##### Extensions
Extensions: `iso`  
Here you put in what extensions Pegasus should look for. In this case it's iso for PS2 games

##### Launch
Launch: `/Applications/PCSX2-v1.7.2952.app`  
This is the path of the app itself, afterwards you can add any type of argument for the emulator in question. Since I'm running the QT version of PCSX2, I could use an argument like `-fullscreen` to have the app launch in full screen mode. You'll need to check the emulators Command Line arguments to know what to put here. `{file.path}` This tells the emulator the filepath of the rom in question.

### Game Data
The next part is how you push your games information to the launcher itself

```
game: Dark Cloud
file: Dark Cloud.iso
developer: Level-5
assets.box_front: assets/covers/dark cloud.jpg
assets.logo: assets/logos/
```
#### Basic Game Info

##### Game
Game: `Dark Cloud`  
tells the launcher what the game title is  

##### File
File: `Dark Cloud.iso`  
tells the launcher what the game file is called. Keep in mind that since this file is placed in the rom directory - there's no need to add any type of file path

#### Extra Game Info
This is extra information that isn't required but will make your titles look nicer

##### Developer
Developer: `Level-5`  
this tells the launcher what developer this is for  

##### Box Front
assets.box_front: `assets/covers/dark cloud.jpg`  
This is the file path and image for the box art front. `jpg` and `png` are supported by Pegasus. Keep in mind that you only need to start from wherever your assets folder begins. So if your assets folder is `cover` for example then it would just be `cover/dark cloud.jpg`  

##### Game Logo
assets.logo: `assets/logos/`  
Similar to the box_front - this is for the logo that will show up on the launcher theme. Not all themes support the logo however.

