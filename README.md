# Princess Sky Escape

## Play the Game
**Unity Play Link**: https://play.unity.com/en/games/e46b08a8-a516-4b73-ac07-78c3262645b5/princess-sky-escape

## Game Overview
Princess Sky Escape is a game where you direct the princess through the sky while trying to avoid the pink sparkly rocks. The objective of this game is to stay away from the flying rocks and borders as long as possible.

### Controls
- Click and drag mouse (laptop/desktop) or finger (mobile device) to move princess in any direction
- Stop pressing and the princess will continue moving in the direction currently moving

### How to Play
To start the game click "Play". After you get to the starting screen you are playing! Beware of this because some of these rocks move fast! The smaller the rock the faster and the bigger the rock the slower. Start by pressing your mouse, if you're on a desktop/laptop, or finger, if you're on a mobile device, and click and hold where you want to go. Once you get the princess moving you can click and drag anywhere you want! Once you stop pressing, the princess will continue to move the direction it was currently going until you click and drag a different direction. You don't want to run into the rocks or the borders! Beware of the rocks as the game goes on... the rocks get faster and faster the higher the score gets.

## Base Game Implementation

### Completion Status
- [x] Player movement and controls
- [x] Obstacle spawning system
- [x] Collision detection
- [x] Score system
- [x] Game over state

### Known Bugs
- The princess is slower when published versus when I developed it and played on Unity Hub.

### Limitations
- Some limitations were that I wasn't able to figure out how to swap out my sprites with custom sprites.

## Extensions Implemented

### 1. Create a Cohesive Color Scheme (2 points)
**Implementation**: I implemented this by having blue as my main color and then having cohesive colors that match well with blue like pink and purple.
**Game Impact**: This changes gameplay because the colors contrast enough for the components to be well identified and it has a more appealing look.
**Technical Details**: Key technical changes included changing the object colors and background colors to match the color scheme.
**Known Issues**: There are no bugs specific to this extension.

### 2. Change Your Entire Game Concept (3 points)
**Implementation**: I implemented this by creating the rocket ship to a princess and then changing the meteors to pink rocks that the princess needs to escape from.
**Game Impact**: This changes gameplay because the princess is trying to escape the pink rocks instead of a rocket ship escaping meteors.
**Technical Details**: Key technical changes included changing the game objects to the desired game concept that I was trying to achieve.
**Known Issues**: There are no bugs specific to this extension.

### 3. Destroy the Borders on Game Over (4 points)
**Implementation**: I implemented this by creating a border parent public game object then when the princess was to run into the borders or the rocks on collision I set the border parent to false.
**Game Impact**: This changes gameplay because when the princess runs into the border or the rocks the borders disappear and the rocks and princess fade out.
**Technical Details**: Key technical changes included creating a border parent game object in the player controller script and on collision making it false so the borders disappear.
**Known Issues**: There are no bugs specific to this extension.

### 4. Add Ambient Background Particles (4 points)
**Implementation**: I implemented this by creating a particle system that continuously loops so the game appears to have dust particles in the background.
**Game Impact**: This changes gameplay because it gives dimension when the game is being played and allows for a nice background.
**Technical Details**: Key technical changes included creating a particle system and setting the emission area, particle size, lifetime, looping, and velocity.
**Known Issues**: There are no bugs specific to this extension.

### 5. Increase Difficulty Over Time (5 points)
**Implementation**: I implemented this by adjusting the speed at which the rocks move as the game goes on, so the higher the score the faster the rocks.
**Game Impact**: This changes gameplay because it makes the game increasingly harder the higher the score gets.
**Technical Details**: Key technical changes included adjusting obstacle physics by setting the PhysMat_Bouncy to 1.05 which allows the obstacles to gain speed with each bounce.
**Known Issues**: There are no bugs specific to this extension.

### 6. Add Sound Effects and Background Music (5 points)
**Implementation**: I implemented this by adding an audio source to the game.
**Game Impact**: This changes gameplay because it makes the game feel like a real game with music playing and it's more engaging.
**Technical Details**: Key technical changes included adding an audio source file to the game and then importing the music track for the game. Then I made the audio looping and reduced the volume to 0.3. 
**Known Issues**: There are no bugs specific to this extension.

### 7. Animate the Booster Graphic with Audio (6 points)
**Implementation**: I implemented this by adding a booster flame when the princess is speeding up and adding an audio source when the booster flame is on.
**Game Impact**: This changes gameplay because it makes the game more exciting, speeding up and allows for the full game experience.
**Technical Details**: Key technical changes included adding a booster flame game object to the princess that is inactive when playing but active when click and drag is implemented. Then I added an audio source file to the booster flame and imported the thruster music track for the booster flame. Then I made the audio looping and reduced the volume to 0.3. 
**Known Issues**: There are no bugs specific to this extension.

## Credits
- Audio tracks from [Unity 2D Beginner Game: Sprite Flight](https://learn.unity.com/course/2d-beginner-game-sprite-flight/tutorial/optional-bonus-features?version=6.0) 

## Reflection
**Total Points Claimed**: [Base: 80% + Extensions: 29% = 109%]
**Challenges**: Some difficult parts of this project was getting familiar with Unity and how all the different parts of 2D games work. I also had trouble with the particle system background and setting it up so the particles themselves weren't big but covered the whole area of the game. I also had trouble deploying my sprite game because I included the sample scene in my deploy and it was just showing a blue screen at first. I was able to fix it by removing the sample scene from the deployment.
**Learning Outcomes**: I learned how to implement 2D game objects and prefabs in Unity with game movements and physics. On top of that I learned how to apply 2D collision detection onto objects and game states. Also, I learned more about Unity's UI system which was intriguing and made the score displays and restart button. Lastly, I learned how to make a 2D game with the extensions that I implemented and deployed. 

## Development Notes
Some additional notes from my development process would be, I had trouble cloning my github repo and committing my game from Unity into that repo. The files were too large.
