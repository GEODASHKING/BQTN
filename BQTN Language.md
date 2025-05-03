1. Declaring Variables
Variables can store positions, actions, or other values, enhancing code reusability.

bqtn
Copy
Edit
var bob = (x: 67, y: 89, ease: "ease-in-out");
var spawn = loop;
var move = (x: bob.x, y: bob.y);
2. Defining Loops
Loops allow for repetitive actions, such as continuous spawning or movement.

bqtn
Copy
Edit
loop = spawn;
spawn = move;
move = loop;
3. Object Movement
Define movement behaviors using variables and loops.

bqtn
Copy
Edit
move = (x: bob.x, y: bob.y, ease: bob.ease);
4. Triggering Actions
Actions can be triggered based on specific conditions or events.

bqtn
Copy
Edit
onPlayerTouch("trigger") {
    // Define actions to perform when the player touches the trigger
}
Example Level Script
bqtn
Copy
Edit
// Define variables
var bob = (x: 67, y: 89, ease: "ease-in-out");
var spawn = loop;
var move = (x: bob.x, y: bob.y, ease: bob.ease);

// Set up looping behavior
loop = spawn;
spawn = move;
move = loop;

// Define actions
onPlayerTouch("trigger") {
    // Actions to perform when the player touches the trigger
}
Getting Started
Install the Bqtn Plugin: Integrate the Bqtn scripting environment into your GD editor.

Write Scripts: Create .bqtn files containing your scripts.

Compile: Use the Bqtn compiler to convert your scripts into GD-compatible formats.

Test: Load your level in GD to test the implemented scripts.

