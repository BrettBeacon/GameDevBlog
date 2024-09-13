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