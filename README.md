# pico_game

Hey guize here's your guide:
This will probably be a shitshow, but I'll be mostly available this week to video chat and help y'all out.

The Basic Idea:
  Github is a version control system that allows us to work on the same files at the same time, essentially.
  The website (github.com) maintains an online repository that you can think of as our "master" file, which we copy
  locally onto our computers for working on. Whenever one of us makes a change that we like, we can send that change
  up to github.com's server where it will apply the change to the online master file. Github will also let you know
  if the changes you make conflict with the changes someone else makes, so you can resolve that issue without overwriting
  other people's stuff.
 
Step 1.
  Make a new folder in whatever directory you keep your carts in ("pico-8/carts") and name that folder whatever you want.
  That's the folder that will be synced with the online repository. Keep it empty for now.
 
Step 2.
  Download Sourcetree (https://www.sourcetreeapp.com/).
  This is the program that we will use to manage the connection with github.com.
  I'm not hugely familiar with it, but it works on both Mac and PC. And it seems easy to use.
  
Step 3.
  Open up Sourcetree and click the "Clone/New" button in the upper left corner.
  In "Source Path / URL:" enter exactly the following: https://github.com/joshuarosen/pico_game.git
  In "Destination Path:" enter the file path for the folder that you made in Step 1, either by typing it in or navigate to
    it using the "..." button.
  Then click the "Clone" button.
  
Step 4.
  There should now be a "game.p8.png" file in that folder.
  You now have a working repository that is linked with the online repo.

Okay, brief description of your basic workflow:
  1. Every time you want to work on the game, you should open up Sourcetree (make sure the repo folder is selected on the left hand side).
  2. Then, you should click the "Pull" button and then click "OK". Pulling means that you are syncing your local folder with the one stored on github.com. This ensures that when you make changes, you're working on the most recent build we have.
  3. After you've pulled, you can go ahead and open up PICO-8.
  4. PICO-8 should initialize to your carts directory. From here, you can type "ls" to see all the files and directories available to you.
  5. Type "cd [your repo folder name]" to change directories to the repo folder. Once again, you can type "ls" to see all the files and directories in this folder (it should only be "game.p8.png" and "README.md")
  6. Then you can load in files with "load game.p8.png"
  7. Now make all your changes. Yay!
  8. When you're done making changes, go back to Sourcetree.
  You should see the file "game.p8.png" in the "Unstaged files" box in the middle of the screen.
  9. Go ahead and click the "Stage All" button which should move the file up to the "Staged files" box.
  Now the file is staged and is ready to be committed.
  10. In the text box towards the bottom of the screen, just under your name/email address, 
    type in a message that says what this change accomplished ("made a new graphic, yay").
  11. Then click the commit button.
  12. It is super important to note that commit does NOT send the changed file to github, it only commits it locally on your machine.
  To send the changed file to github.com, you have to click the "Push" button AFTER you stage and commit the file.
  13. Make sure the "master" branch is checked in the popup window, and then click the second "Push" button to send the file to github.com
  Now the changed file will be on github.com and when someone else clicks the "Pull" button they will get the newly changed file.
  
  
  
  
  
