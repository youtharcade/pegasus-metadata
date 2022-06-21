# Explanation of PS2 Setup

## Metadata Start
The first piece of information the metadata needs is the Collection/Launch data

#### Collection Information

``
Collection: Playstation 2
Shortname: PS2
Extensions: iso
Launch: /Applications/PCSX2-v1.7.2952.app {file.path} 
``

// You can add as many extensions as you want by adding a comma but keep in mind the emulator has to support it
// When you launch the emulator - you can add arguments, but they have to go between the application and file path
// This is where you add your games - Pegasus will find every game within the folder, however there will be no metadata.
// There's many different ways to get the metadata, I'm coding it by hand for the practice. You can use a scraper if you'd like.
// For more information on that aspect, you'll need to hit up the Pegasus website: https://pegasus-frontend.org/docs/user-guide/meta-assets/
// game name
// rom file name
// Developer name
// Box front asset - the easiest way to do this is to create an asset folder in your PS2 rom folder
// Logo asset - some themes use this information
