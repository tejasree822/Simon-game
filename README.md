# Simon-game
A Simon memory game built using HTML, CSS, JavaScript and jQuery
Simon Game 🎮

A browser-based memory game inspired by the classic Simon Game. The player must repeat an increasingly long sequence of colors and sounds. The game continues until the player makes a mistake.

How to Play
Press any key to start the game.
A random button will flash and play a sound.
Click the button that was shown.
Each new level adds one more color to the sequence.
Repeat the entire sequence in the correct order.
If you click the wrong button, the game ends.
Press any key to restart.
Features
Random sequence generation
Sound effects for each button
Button press animations
Level tracking
Game-over detection
Restart functionality
Technologies Used
HTML
CSS
JavaScript
jQuery
Project Logic
Game Start
The game waits for the first key press.
A started flag prevents the game from starting multiple times.
The first call to nextSequence() begins the game.
Sequence Generation
A random color is selected from:
Red
Blue
Green
Yellow
The selected color is added to the gamePattern array.
The corresponding button flashes and plays a sound.
User Input
Every button click is stored in the userClickedPattern array.
The clicked button plays its sound and shows a press animation.
Answer Validation
After each click, the latest user input is compared with the corresponding element in gamePattern.
If the input is correct, the game continues.
If all inputs for the current level are correct, a new sequence is generated.
Game Over
If the user clicks the wrong button:
A "wrong" sound is played.
A game-over animation is shown.
The title changes to indicate the game has ended.
Game variables are reset and the player can restart by pressing any key.
Future Improvements
Add a high-score tracker.
Add difficulty levels.
Add mobile touch support.
Store best scores using local storage.
