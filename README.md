# Colonial Pirate Parkour Unity Project
#### Video Link: https://youtu.be/qN9pwBX1enA
#### Description: 
I was inspired by Assassin's Creed Black Flag when I found a Colonial Map and a Pirate Asset 
and thought it would be fitting for the Dynamic Parkour Plugin I was going to use.
Hence, this project is a third-person parkour Project built in Unity, written in C#
which is what the Dynamic Parkour Plugin uses.

While the Video above does have a voice over, I'll describe it here.
As you can hear, I've added music from Assassin's Creed Black Flag to give
it more of that Pirate ambience to it because we start climbing up the building.
We eventually reached the top, where our character pulled themselves atop the building.
We then actually jump into the tower of the building before jumping back out to the beginning.

Then we go into the graveyard, where we sprint into it, where there's a noticeable increase in speed
when running. I then proceed to show our character vaulting over the wall multiple times, back and forth.
This leads us to jump over the graves or climb atop them, and sometimes we climb atop the tombstones and even parkour between them.
We then go towards the back of the map, where we slide under a block before climbing up some stairs to the top of the building.

We then run to the same building, different location and climb up it like we did with the church before jumping through the building again and ending at the beginning.

## Design Choices
Adapted A Colonial Map and Pirate Character to work with the Parkour Plugin
Display actions of Climbing, Sliding, Jumping, Vaulting, Running, and Reaching
Inspired by Assassin's Creed Black Flag, hence given the setting and character
Added music from the game to make things feel more immersive.
## Structure
Everything that matters is stored in the Assets Folder
**Assets/Colonial City LittlePack** - This includes the actual map I used in the video with all of the objects and the scene where the video took place.
**Assets/Dynamic Parkour System** - This is where the Dynamic Parkour Plugin is, along with its scripts. I had to reference this folder many times to adapt the map and the character
**Assets/Pirate** - This is where the Pirate Character is located
Also in the Assets Folder is the soundtrack itself, which I put in the background

## Challenges and Learning
There were many Challenges and Points of Learning for this. So I'll be going in Order
**Material Problems**
My first issue was when loading the assets into Unity, they had no Materials attached. What that meant was when I loaded each asset for the first time, they were light pink or light blue.
I eventually figured this out and had to add materials to each GameObject, and eventually, each asset looked like how they were displayed on the Asset Stor.e

**Parkour Problems**
This is where most of my time went. There were several parkour issues. I'll divide this section further to explain
- Character
I was using a different character when it came to what was given in the plugin, now, while the developer did make a video showing how to use the plugin.
I did struggle a bit to put my Pirate character atop the rigged character in the Testing Scene for the Plug In; I'd have to go to this scene multiple times.
Eventually, I managed to figure out how to add my character and make it move, incorporating my adjustments.

- Climbing
This took up the most time by far. First, I had to add colliders for the Church, then I went about adding ledges to climb up onto the church.
The main issue was that I could get my character to climb the first block, but they couldn't climb the 2nd or the 3rd.
This led me to dive into the Plugin's scripts to see whether I could adjust the height I jump or make it so I could jump to the next block. I even looked at the developer's ReadMe and Documentation to find something.
It took like a few days to figure out, but eventually I did manage to get it working using an alternative, which meant I would apply it and test it around the map.

- Vaulting and Jumping
Figuring out the Climbing portion took a huge weight off my chest, now it was to deal with adding in places to Vault and Jump. I had already added some Jumps to get my mind off the Climbing issue
But even this had issues. While I could jump from the top to the bottom, I couldn't jump from side to side, which is where I realised, when reading the documentation, that it's basically on
directional values. Essentially, where the arrow faces. So I had to rotate the objects and or change their scale to be able to jump over the graves. I also did similar adjustments when it came to
Reaching/Climbing Up on some graves and tombstones, as I had to adjust their scale to make my character able to climb up the tombstone. I did the same adjustments on the walls, making them small
enough to vault over when needed.

**Sliding and Reaching**
These two things weren't much of an issue, but I knew I had to display them. The only climbing issue I had was that once I got to the top of one of the buildings.
I couldn't jump onto the building, which led me to adjust their box colliders to make it able to jump onto the building and also make it so I wasn't floating.
When on the building. 

## Reflection
This project taught me a lot of things to improve on or explore in the future
- Using a third-party Unity Plugin to adapt to a completely different environment
- Being able to set up and rig my character atop another Rigidbody
- Adjusting Unity's colliders, materials and meshes using the Inspector extensively
- Reading the C# script of the third-party plugin to understand what's wrong and what's at play
- Finding alternative solutions to the problems presented and eventually coming to a finished project
- 
## Due to Size Limitations, Some files were compressed outside of their respective larger folders
Such as the Graveyard Textures for the Colonial City
The TGA converted PNGs for the Pirate
and the zipped Animations and Textures for the Dynamic Parkour Plugin
