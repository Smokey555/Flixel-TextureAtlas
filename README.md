# Flixel-TextureAtlas
 
 Very experimental Flixel implementation for Animate 2018 (2018 ONLY RIGHT NOW!) TextureAtlas. Mostly a fork of [Original](https://github.com/miltoncandelero/OpenFLAnimateAtlas).

 ## Credits / shoutouts

 - [Smokey](https://twitter.com/Smokey_5_)
 - [Rozebud](https://twitter.com/helpme_thebigt)
 - [miltoncandelero](https://github.com/miltoncandelero) (Original Code)

 Current changes done to the original Code:
 Flixel Implementation
 BlurEffect support
 Some very minor fix stuff

  ## Usage/Current Limitations

  This is a very early build, but it works(kinda), so there's a few limitations, including:
  -Animate 2018 Only (i don't fucking know why)
  -Not all Animate Effects are working yet(BlurEffect works, but GlowEffect etc. doesn't, also very laggy)
  -Generated bitmaps cut off sometimes(Might be able to fix that soon)

  How to do the thing:
  Make a movieclip in Animate, put all animations with their frames in there. Then, click on the first frame of each animation, go to "Properties", and give the animation a label. That label will be the animation name.

  Usage in Flixel is made as easy as possible, you give it to a Sprite just like a normal Spritesheet animation:

 `sprite.frames = AtlasFrameMaker(Path,widthoffset,heightoffset,excludeArray)`
 
 Path is the path to the folder that's generated by Animate(duh).
 Width- and Heightoffset are a temporary fix to the cutting off bitmap issue(I'm trying to fix it rn gimme a bit).
 excludeArray excludes animations from being created. Let's say you have 2 GF versions on 1 TextureAtlas, you could exclude the animations from the one that you don't need currently,making it load faster.

 ALSO MAKE SURE TO ALIGN THE ANIMATIONS YOU PLACE TO LEFT AND TOP USING "ALIGN" IN ANIMATE! There's an example .fla so you can see what you gotta do.

    
