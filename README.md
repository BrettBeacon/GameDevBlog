# GameDevBlog

## Week 1
First week back for semester 2!

## Week 2
Week 2 of the semester and we are full steam ahead into getting things done. This week, me and the team worked on getting the game project questions answered, inputting what we wanted to get done this semester into the timeline gantt, setting up trello and making a commitment to actually using it and finally, getting the template completed for the project pitch deck.  

The timeline gantt for semester 2 with a breakdown of the things we want to try and implement:

![Timeline Gantt for Semester 2](/Timeline_Gantt.PNG "Timeline Gantt")

This is the Trello board set up for semester 2, however, it is still bare bones and needs more work:

![Trello Board for Semester 2](/Trello_Board.PNG "Trello Board")

So far, week 2 has been fairly productive, each of the team members have put in some good work in getting these documents ready, and we have also worked with Tom on a logo design for the game, he has done amazing work and we are all very happy with the logo design chosen.  

## Week 3
Week 3 was focused on finishing the pitch deck draft and other documents required for submission. We had added the remaining information we wanted to showcase in the pitch deck, and tried to adapt it to both the work required for university and what we want to do with the project after university.  

Tom was able to come up with some mock up posters and some more materials that we ended up using as the background in the slides, as well as colouring the pitch deck to fit a theme. The final draft poster has some changes from the mock up Tom was able to come up with, but it is a improvement and fits the theme perfectly.

This is the poster Tom was able to mock up for the game and game title with the nuclear green theme. 

![Dead Pine Village Poster Draft](/DeadPine_KeyArt_Draft.jpg "Game Poster")

## Week 4
Week 4 was when we presented our pitch deck to the class. I am super happy with the work that was put in, and considering it is just a draft, it has turned out really nice. We can now start to fill it out with the content that we make through the weeks and get it ready for the final presentation.  

This was also the start of sprint 2, however, I have started working on the implementation of the weapons system, along side the animations and movement required for this, ideally, this was meant to be started back in the end of sprint 1, according to the timeline gantt we had set up, but things just got ahead of me, and I have had to move it to starting in sprint 2.  

I have researched on how I might best achieve what I want for the shooting and weapons system, and found some interesting ways of achieving it, however, it also means I will need to start from scratch with the character movement system, as at this stage, what is currently implemented will directly clash with how the new system will be set up.  

Just a reminder of where we are starting, and hopefully, in another 8-10 weeks, the differences will be massive.  

![Dead Pine Village Current State](/Overview.PNG "Overview")

## Week 5
Where are the weeks going?!?! End of week 5 already, end of sprint 2, god damn it, time seems to fly.  

I have started implementing the new movement system with weapons and guns in mind, I have made a new scene to work in so I'm not having to go through menus and what not for testing purposes. I also implemented a new character model from the Unity Asset store just so I can play around with the animation rigging system in Unity, and adding weapons to hand slots. This wasn't possible with the current character model from Daniel, as I didnt have a version of him in a T-Pose, which I need for animation purposes. Daniel is also redesigning the hero character anyway, so using a new model isnt a big deal at this stage.  

There is a lot of work to be done, and time seems to go faster than you remember, especially when you need to get things done.

## Week 6
In week 6, I was able to get more of the animation and rigging completed for the new shooting system. It is a new system that I haven't used before, but following a tutorial has helped me to implement it into the game quiet easily. The new system uses the Unity animation rigging system, it has multi-bone IK constraints which help to make sure the arms of the player are attached to the weapon, which makes it easier to move the weapon around without having to move the arms indenpentantly, saving on a lot of work. I have implemented the character holding the weapon in a position that makes sense for running. Further animations will be added for aiming.  

![New Animation Rigging System T-Pose](/Week5_NewCharacterRigging&Animation.PNG "T-Pose")
![New Animation Rigging System Running Pose](/Week5_NewCharacterRigging&Animation_InPose.PNG "Pose")
![New Animation Rigging System Running Pose Behind](/Week5_NewCharacterRigging&Animation_InPoseBack.PNG "Pose Behind")

I have also implmeneted new animations for the running that work in a 8 directional axis, which is an improvement upon the old running animation, which would slide when going side to side. The new animations use a blend tree that increases the speed based on the buttons pressed.  

![New Animation Rigging System Running](/NewCharacterMovement.gif "Running Animations")

## Week 7
Week 7 was a continuation of implementing more animations and rigging to help better control the characters shooting. This week, I focused on getting the aiming system working with the animations, and making sure the character's animations follow where the player is aiming. This builds on top of the animations and rigging system already implemeted in week 6.  

![Aiming Rigging System](/NewCharacterMovementAiming.gif "Aiming")  

This works by using a multi-constraint aiming rig which uses the Spine1, Spine2 and Head bones to rotate when the aim is moved, allowing a realistic look of movement. The aiming is also controlled using right mouse click, this allows the animation to be help in a hold position while running, then change to an aiming position when the player wants to aim.

## Week 8
The start of week 8, my focus this week will be adding more on top of the animation and rigging system, implementing shooting and picking up weapons.  

During Week 8, I also received the skeleton crops / growth cycles from Alex, one of the 3D artists working on the game. There are a total of 4 growth cycles, however, I already had the final cycle in the form of the skeleton monster model, I just needed the 3 that came before it. Now I have them, I have changed over the carrot seed data in the game to now show the skeleton growth cycle models instead of the carrots growth cycles. The first growth, or the seedling stage is a skeleton skull and two bones on the soil, after the player waters this and the day clicks over, the next stage will show, which is the skeleton's hand raising out of the ground with his head as well, and the third stage is the skeleton trying to pull himself out of the ground. The final stage of growth is the full skeleton standing on the ground ready to be released and for the player to shoot and fight for loot.

Here is a rapid GIF of the planting and growing in action:

![Skeleton Monster Growing](/MonsterGrowingDemo.gif "Monster Growing of Skeleton")

## Week 9
Week 9 was a continued effort to get more of the weapon system in place. My focus is still to implement a robust weapons system that can go a long with the farming system that is already in place.  

During weeks 8 and 9, I implemented a change with the shooting, from an instant raycast shot to a bullet being rendered with a tracer.

![Raycast Shooting with Tracer](/RaycastShootingWithTracer.gif "Raycast shooting with tracer")

I was also able to get a muzzle flash added to the weapon and on hit effects for when a bullet hits a surface. There are different on hit effects available, but at this stage, I am only using one. It could be changed later to detect what it is hitting and change the hit effected based on that, for example, when shooting a slime, the hit effect could be changed to a slime hit effect instead of the current metal hit effect.

![Muzzle Flash](/MuzzleFlashWeaponAiming.gif "Muzzle Flash with Weapon Aiming")

And finally, I also added in bullet drop, bullet speed and the rate of fire which can be changed in the inspector for further adjustment based on the weapon in use.

![Bullet Render with Drop](/BulletRenderWithDrop.gif "Bullets being rendered with bullet drop")

## Break Week
Over the break week, I was starting to receive a lot of the models and other works from the team, so as a part of my job within the engine, I imported all the models and fixed up their materials and added in the animations.

There was some issues with the importing and figuring out what settings were best for each of the assets, especially the slime as it was designed to be transparent.

![Slime Opaque Test](/Slime_Opaque_Test.png "Opaque slime after importing before settings were changed")

![Material Settings](/Material_Settings.gif "Changing the settings from opaque to transparent")

After finding the change in the material settings, it was clear I was able to achieve the transparent look we wanted from what was designed from the 3D artists.

![Transparent Settings](/Transparent_Material_Settings.gif "Changing the transparent settings to see the differences")

As you can see above, there were some differences within the transparency settings, however, we stuck with the alpha channel with alpha clipping turned off. Alpha clipping was an option I thought would help to show the transparent look of the slime, and originally thought this was the solution, but when I found the transparent setting, it was clear alpha clipping was not a good choice.  

So the slime went from this:

![Opaque Slime](/Slime_Opaque_Test.png "Opaque Slime")

to this:

![Transparent Slime](/Slime_Transparent_Final.png "Transparent Slime")

This is a much better look and feels like an actual slime monster.

I was also able to import the other assets and add their materials and textures too.

![Seeds](/Seeds_Test.png "A line up of all the seeds")
![Slime Seed Transparent](/Slime_Seed_Transparent_Final.png "Fixing the slime seed to match the transparent look of the slime")
![Slime & Crops with Transparent](/Slime_and_Crops_Transparent_Final.png "Final look of slime and crops")
![Spider Crops](/Spider_Crop_Final.png "Spider crops for each growth stage")
![Overall Look in Game](/Asset_Import_In_Game.png "An overall look of the assets in game")

I was also able to import the animations of the Slime into Unity and hook them up to demo. I have only added in the attacking animation at this stage, but there is also a walking animation that I will show in Week 10.

![Slime Attacking Animation](/Transparent_Slime_Attacking_Animation.gif "Slime Monster Attacking")

Finally, in the break week, I was able to implement some weapon pick up, at this stage, it is implemented using spheres in the world that the player walks over to change weapon, however, this will be changed to a weapon selector wheel in week 10 or 11. There were also changes to the animation system as the player starts off with no weapon, so their hands are by their side, but when they run into a weapon, they pick it up and the animations and Hand IKs change to suit that weapon.  

This was done by implementing animation capture code that allows me to set where the hands and gun are and capture the settings to be saved for the future without losing it when the game stops.

![Weapon Pickup In Game](/Weapon_Pickup_Custom_Animation.gif "Weapon pickup in game")

Here is the view from the editor viewport for a better look at how the animation changes for each weapon.

![Weapon Pickup Editor Viewport](/Weapon_Pickup_Custom_Animation_Editor_Viewport.gif "Editor viewport version of weapon pickup")

The systems and game are coming a long nicely, we are certainly behind on our timeline gantt, but I think we will have enough time to put all the systems together to showcase a short demo of the crops growing, the monsters being released and walking towards the player, the player shooting and killing the monsters and having multiple weapons to do it.

## Week 10