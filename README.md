# GameDevBlog

## Week 1
First week back for semester 2!

## Week 2
Week 2 of the semester and we are full steam ahead into getting things done. This week, me and the team worked on getting the game project questions answered, inputting what we wanted to get done this semester into the timeline gantt, setting up trello and making a commitment to actually using it and finally, getting the template completed for the project pitch deck.  

The timeline gantt for semester 2 with a breakdown of the things we want to try and implement:

![Timeline Gantt for Semester 2](/Resources/Timeline_Gantt.PNG "Timeline Gantt")

This is the Trello board set up for semester 2, however, it is still bare bones and needs more work:

![Trello Board for Semester 2](/Resources/Trello_Board.PNG "Trello Board")

So far, week 2 has been fairly productive, each of the team members have put in some good work in getting these documents ready, and we have also worked with Tom on a logo design for the game, he has done amazing work and we are all very happy with the logo design chosen.  

## Week 3
Week 3 was focused on finishing the pitch deck draft and other documents required for submission. We had added the remaining information we wanted to showcase in the pitch deck, and tried to adapt it to both the work required for university and what we want to do with the project after university.  

Tom was able to come up with some mock up posters and some more materials that we ended up using as the background in the slides, as well as colouring the pitch deck to fit a theme. The final draft poster has some changes from the mock up Tom was able to come up with, but it is a improvement and fits the theme perfectly.

This is the poster Tom was able to mock up for the game and game title with the nuclear green theme. 

![Dead Pine Village Poster Draft](/Resources/DeadPine_KeyArt_Draft.jpg "Game Poster")

## Week 4
Week 4 was when we presented our pitch deck to the class. I am super happy with the work that was put in, and considering it is just a draft, it has turned out really nice. We can now start to fill it out with the content that we make through the weeks and get it ready for the final presentation.  

This was also the start of sprint 2, however, I have started working on the implementation of the weapons system, along side the animations and movement required for this, ideally, this was meant to be started back in the end of sprint 1, according to the timeline gantt we had set up, but things just got ahead of me, and I have had to move it to starting in sprint 2.  

I have researched on how I might best achieve what I want for the shooting and weapons system, and found some interesting ways of achieving it, however, it also means I will need to start from scratch with the character movement system, as at this stage, what is currently implemented will directly clash with how the new system will be set up.  

Just a reminder of where we are starting, and hopefully, in another 8-10 weeks, the differences will be massive.  

![Dead Pine Village Current State](/Resources/Overview.PNG "Overview")

## Week 5
Where are the weeks going?!?! End of week 5 already, end of sprint 2, god damn it, time seems to fly.  

I have started implementing the new movement system with weapons and guns in mind, I have made a new scene to work in so I'm not having to go through menus and what not for testing purposes. I also implemented a new character model from the Unity Asset store just so I can play around with the animation rigging system in Unity, and adding weapons to hand slots. This wasn't possible with the current character model from Daniel, as I didnt have a version of him in a T-Pose, which I need for animation purposes. Daniel is also redesigning the hero character anyway, so using a new model isnt a big deal at this stage.  

There is a lot of work to be done, and time seems to go faster than you remember, especially when you need to get things done.

## Week 6
In week 6, I was able to get more of the animation and rigging completed for the new shooting system. It is a new system that I haven't used before, but following a tutorial has helped me to implement it into the game quiet easily. The new system uses the Unity animation rigging system, it has multi-bone IK constraints which help to make sure the arms of the player are attached to the weapon, which makes it easier to move the weapon around without having to move the arms indenpentantly, saving on a lot of work. I have implemented the character holding the weapon in a position that makes sense for running. Further animations will be added for aiming.  

![New Animation Rigging System T-Pose](/Resources/Week5_NewCharacterRigging&Animation.PNG "T-Pose")
![New Animation Rigging System Running Pose](/Resources/Week5_NewCharacterRigging&Animation_InPose.PNG "Pose")
![New Animation Rigging System Running Pose Behind](/Resources/Week5_NewCharacterRigging&Animation_InPoseBack.PNG "Pose Behind")

I have also implmeneted new animations for the running that work in a 8 directional axis, which is an improvement upon the old running animation, which would slide when going side to side. The new animations use a blend tree that increases the speed based on the buttons pressed.  

![New Animation Rigging System Running](/Resources/NewCharacterMovement.gif "Running Animations")

## Week 7
Week 7 was a continuation of implementing more animations and rigging to help better control the characters shooting. This week, I focused on getting the aiming system working with the animations, and making sure the character's animations follow where the player is aiming. This builds on top of the animations and rigging system already implemeted in week 6.  

![Aiming Rigging System](/Resources/NewCharacterMovementAiming.gif "Aiming")  

This works by using a multi-constraint aiming rig which uses the Spine1, Spine2 and Head bones to rotate when the aim is moved, allowing a realistic look of movement. The aiming is also controlled using right mouse click, this allows the animation to be help in a hold position while running, then change to an aiming position when the player wants to aim.

## Week 8
The start of week 8, my focus this week will be adding more on top of the animation and rigging system, implementing shooting and picking up weapons.  

During Week 8, I also received the skeleton crops / growth cycles from Alex, one of the 3D artists working on the game. There are a total of 4 growth cycles, however, I already had the final cycle in the form of the skeleton monster model, I just needed the 3 that came before it. Now I have them, I have changed over the carrot seed data in the game to now show the skeleton growth cycle models instead of the carrots growth cycles. The first growth, or the seedling stage is a skeleton skull and two bones on the soil, after the player waters this and the day clicks over, the next stage will show, which is the skeleton's hand raising out of the ground with his head as well, and the third stage is the skeleton trying to pull himself out of the ground. The final stage of growth is the full skeleton standing on the ground ready to be released and for the player to shoot and fight for loot.

Here is a rapid GIF of the planting and growing in action:

![Skeleton Monster Growing](/Resources/MonsterGrowingDemo.gif "Monster Growing of Skeleton")

## Week 9
Week 9 was a continued effort to get more of the weapon system in place. My focus is still to implement a robust weapons system that can go a long with the farming system that is already in place.  

During weeks 8 and 9, I implemented a change with the shooting, from an instant raycast shot to a bullet being rendered with a tracer.

![Raycast Shooting with Tracer](/Resources/RaycastShootingWithTracer.gif "Raycast shooting with tracer")

I was also able to get a muzzle flash added to the weapon and on hit effects for when a bullet hits a surface. There are different on hit effects available, but at this stage, I am only using one. It could be changed later to detect what it is hitting and change the hit effected based on that, for example, when shooting a slime, the hit effect could be changed to a slime hit effect instead of the current metal hit effect.

![Muzzle Flash](/Resources/MuzzleFlashWeaponAiming.gif "Muzzle Flash with Weapon Aiming")

And finally, I also added in bullet drop, bullet speed and the rate of fire which can be changed in the inspector for further adjustment based on the weapon in use.

![Bullet Render with Drop](/Resources/BulletRenderWithDrop.gif "Bullets being rendered with bullet drop")

## Break Week
Over the break week, I was starting to receive a lot of the models and other works from the team, so as a part of my job within the engine, I imported all the models and fixed up their materials and added in the animations.

There was some issues with the importing and figuring out what settings were best for each of the assets, especially the slime as it was designed to be transparent.

![Slime Opaque Test](/Resources/Slime_Opaque_Test.png "Opaque slime after importing before settings were changed")

![Material Settings](/Resources/Material_Settings.gif "Changing the settings from opaque to transparent")

After finding the change in the material settings, it was clear I was able to achieve the transparent look we wanted from what was designed from the 3D artists.

![Transparent Settings](/Resources/Transparent_Material_Settings.gif "Changing the transparent settings to see the differences")

As you can see above, there were some differences within the transparency settings, however, we stuck with the alpha channel with alpha clipping turned off. Alpha clipping was an option I thought would help to show the transparent look of the slime, and originally thought this was the solution, but when I found the transparent setting, it was clear alpha clipping was not a good choice.  

So the slime went from this:

![Opaque Slime](/Resources/Slime_Opaque_Test.png "Opaque Slime")

to this:

![Transparent Slime](/Resources/Slime_Transparent_Final.png "Transparent Slime")

This is a much better look and feels like an actual slime monster.

I was also able to import the other assets and add their materials and textures too.

![Seeds](/Resources/Seeds_Test.png "A line up of all the seeds")
![Slime Seed Transparent](/Resources/Slime_Seed_Transparent_Final.png "Fixing the slime seed to match the transparent look of the slime")
![Slime & Crops with Transparent](/Resources/Slime_and_Crops_Transparent_Final.png "Final look of slime and crops")
![Spider Crops](/Resources/Spider_Crop_Final.png "Spider crops for each growth stage")
![Overall Look in Game](/Resources/Asset_Import_In_Game.png "An overall look of the assets in game")

I was also able to import the animations of the Slime into Unity and hook them up to demo. I have only added in the attacking animation at this stage, but there is also a walking animation that I will show in Week 10.

![Slime Attacking Animation](/Resources/Transparent_Slime_Attacking_Animation.gif "Slime Monster Attacking")

Finally, in the break week, I was able to implement some weapon pick up, at this stage, it is implemented using spheres in the world that the player walks over to change weapon, however, this will be changed to a weapon selector wheel in week 10 or 11. There were also changes to the animation system as the player starts off with no weapon, so their hands are by their side, but when they run into a weapon, they pick it up and the animations and Hand IKs change to suit that weapon.  

This was done by implementing animation capture code that allows me to set where the hands and gun are and capture the settings to be saved for the future without losing it when the game stops.

![Weapon Pickup In Game](/Resources/Weapon_Pickup_Custom_Animation.gif "Weapon pickup in game")

Here is the view from the editor viewport for a better look at how the animation changes for each weapon.

![Weapon Pickup Editor Viewport](/Resources/Weapon_Pickup_Custom_Animation_Editor_Viewport.gif "Editor viewport version of weapon pickup")

The systems and game are coming a long nicely, we are certainly behind on our timeline gantt, but I think we will have enough time to put all the systems together to showcase a short demo of the crops growing, the monsters being released and walking towards the player, the player shooting and killing the monsters and having multiple weapons to do it.

## Weeks 10, 11 and 12
During the 3 weeks after the break week, it was my goal to start bringing the game together, moving the things I worked on during the semester over to the original farm scene and start to build it out into a gameplay loop. While I wanted to stop production of anything new eventually, I worked on a few things in weeks 10 and 11, which mainly consist of implementing the weapon wheel system and improving the terrain.

The weapon wheel was fairly simple to implement, however, hooking it up to the weapon pick up system proved to be a little challenging, although not impossible. Eventually, I was able to get the weapon wheel to act like the weapon pick up and the player is able to choose their weapon in the wheel. While there were some challenges, like ensuring there was a visible cursor when the weapon wheel was visible, making sure the cursor didn't impact the already implemented inventory system, and making sure the camera didn't move when the wheel was open, and finally, making sure the gun you selected didnt fire when clicking. All of this was achieved, however, there is still a small bug with the camera and the player when the weapon wheel or inventory is open, and that is when the inventory or weapon wheel is open, the camera is frozen in place, but the player can still move the character in the scene. This minor bug will be fixed at some point in the future, but not at this stage as it is not important enough to fix.

![Weapon Wheel Selector](/Resources/NoShootingNoCameraMoveInventory.gif "Weapon Wheel working with no shooting")

The other thing I worked on during these few weeks was implementing a better terrain system as well as adding in grass textures, grass terrain layer and a tree spawner. We had some problems in the beginning with the terrain, firstly we had just selected a brownish texture for the terrain layer to act as "dirt", however, after seeing this in action, we decided it didn't look good. We eventually changed it to a 2D grass texture that can sit on the terrain layer, this looked much better and helped to blend the 3D grass into the terrain. 

Some other problems we had was with the 3D grasses we were using, and the trees we were using as well. The 3D trees we used in the tree paint brush tool were too high poly, and after spawning ~1000 of them, it slowed the game down way to much. We eventually fixed this by using a different tree we had, however, this new tree isn't as good looking, but for now, it works and does the job. 

We also had a similar problem with the grass, however, this problem was happening when we still had the old tree, and it turns out the tree was the problem all along, however, I still changed the grass to an asset found on the Unity asset store that was specifically built for the terrain system. There is still a minor bug with the grass though, and that is the grass looks black before light hits it, this seemingly only happens after alt tabbing, as when first loading the Unity engine, the grass looks normal, it was only when I alt tabbed to a different program, that the grass would then turn black in the editor, and would stay black until light from the directional light object would hit it, then showing its true colour.

![Grass changing colour with light](/Resources/GrassChangingColourWithLight.gif "Grass changing colour with light")

I was also able to do a small mock up of what the farming might look like when filled out a decent amount, while these images show the same monster over the growth cycles, try to imagine different monsters in the different plots.

![Monster Farming](/Resources/Aerial_View_Farm_Before_Seed_Change.PNG "Aerial View of the farm layout")

The screenshots here are before any of the desired changes, as you can see, the first stage is still the orange mound, this will be changed at a later date.

![Monster Farming Stage 1](/Resources/Skeleton_Seedling_Stage_Demo.PNG "Monster Farming Stage 1")
![Monster Farming Stage 2](/Resources/Skeleton_Sapling_Stage_Demo.PNG "Monster Farming Stage 2")
![Monster Farming Stage 3](/Resources/Skeleton_Third_Stage_Demo.PNG "Monster Farming Stage 3")
![Monster Farming Stage 4](/Resources/Skeleton_FInal_Stage_Demo.PNG "Monster Farming Stage 4")

The four cycles of the skeleton monster crop, not all monsters will be 4 stages, some will be less, some maybe more, this can be changed quiet easily in the game due to the way the seed data is set up.

## Beyond
While officially, the 12 weeks of university program has ended, the games course usually gives extended assignment due dates due to the nature of making a game being incredibly difficult. This gives us more time beyond the due date of this assignment that documents what we had made during the semester, however, I would like to talk about what is left to do in the game to get it in a position I think is acceptable for submission and to show a small gameplay loop.

- Enter all the seed data with the monsters
- Change the first cycle of planting from the orange mound to a seed specific to the monster being planted
- Release the monsters when they are at their final stage
- Add a health system in so the player can kill the monsters
- Ensure the monsters are added to the navmesh when released and the navmesh is working correctly
- Add in debug buttons to help control the flow of time and the growing stages
- Add in the animations of all the monsters
- Add in any assets that haven't been so far

There is still a lot to do, and so little time to do it in, at this stage, I think the important stuff will be handled first, but ideally, the entire list should be completed before submission. All of this is on top of finalising other assignment work in other classes, as well as getting the final pitch deck complete, the presentation slides done, and writing up scripts for what we want to say and who is gonna say it for both pitch deck and presentation!

## After University
There is so much more I would love to do with this game after university, and I really hope I will have the time and means to continue working on this game for the foreseeable future. I have applied for one of the 3-4 grants I would like to get, which would help achieve finishing the game, but these things aren't guaranteed, so we will see, maybe it will just be a part time project that I continue to work on solo outside of finding a job, either in the games industry or not.