# infinityball
A project where the player is a ball that infinitly moves forward.
The player must avoid other automatically spawned obstacles by moving to sides.

## Goal of the game
Goal of the game is to play for as long as possible by avoiding the obstacles to score points.

## Getting Started
1) Entering the game
2) Building the game

## 1) Entering the game
Editor - load scene "scene_0" from the scene folder and click the play button in editor
        
### Start the game
First scene (scene_0) is the "Main Menu" scene. To play the game just press "Play" button.
Second scene (scene_1) is the gameplay scene.

### Pause the game
To pause the game, click on the "Pause" button at upper right corner of the screen.
To resume the game click the "Resume" button.
To restart the game click the "Restart" button.
To go back to Main Menu click the "Main Menu" button.

### Controls
Editor:
- keyboard (A) - move left
- keyboard (D) - move right

Android build:
- tilt device left and right to move left and right

### Gameplay
Main character of the game is the ball.
The ball keeps moving forward until it hits an obstacle.
Once the ball hits an obstacle, the camera will move to the side of the ball and in a few seconds the game over screen will be activated.

### Scoring system
Game scoring system is simple.
Player earns points by avoiding the obstacles.
How many points the player earns can be modified from the editor, find game object "ScoreManager" and change variable "Score Increment".

### Spawn system
Obstacles are spawned from the "SpawnEnemyManager" game object and same named script under that game object.
Obstacles are placed in a List<GameObject> so we can recycle them to save resources.
Obstacles are spawned every few seconds (modify from the editor)

## 2) Building the game
Game is preset to work with Android 4.0 and above

To build the game for android, at the top left corner of the unity editor, click on the "File" button.
After, click on the "Build Settings" button.

You can click the "Player Settings" button in the newly opened window to change build settings but you don't have to as everything's set to work with Android phones.
To build the APK, click the "Build" button.
If you don't want to build it, there's a prebuilt APK included in the project folder "Apk"
        - place the file anywhere inside your phone, install it and open it once it's installed
