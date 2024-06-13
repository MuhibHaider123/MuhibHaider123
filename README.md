I'd love to help, but I cannot send you the entire coding for a Spider-Man game. However, I can provide some guidance on how to create a simple Spider-Man game using HTML, CSS, and JavaScript.

Here's a basic example to get you started:

HTML:
```
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Spider-Man Game</title>
	<link rel="stylesheet" href="style.css">
</head>
<body>
	<div class="game-container">
		<div class="spider-man"></div>
		<div class="obstacles"></div>
		<div class="score"></div>
	</div>
	<script src="script.js"></script>
</body>
</html>
```
CSS (in style.css file):
```
.game-container {
	width: 500px;
	height: 500px;
	border: 1px solid black;
}

.spider-man {
	width: 50px;
	height: 50px;
	background-color: red;
	border-radius: 50%;
	position: relative;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}

.obstacles {
	width: 50px;
	height: 50px;
	background-color: blue;
	position: absolute;
	top: 100px;
	left: 100px;
}
```
JavaScript (in script.js file):
```
const spiderMan = document.querySelector('.spider-man');
const obstacles = document.querySelector('.obstacles');

document.addEventListener('keydown', (event) => {
	if (event.key === 'ArrowUp') {
		spiderMan.style.top = `${spiderMan.offsetTop - 10}px`;
	}
	if (event.key === 'ArrowDown') {
		spiderMan.style.top = `${spiderMan.offsetTop + 10}px`;
	}
	if (event.key === 'ArrowLeft') {
		spiderMan.style.left = `${spiderMan.offsetLeft - 10}px`;
	}
	if (event.key === 'ArrowRight') {
		spiderMan.style.left = `${spiderMan.offsetLeft + 10}px`;
	}
});

// Add obstacle movement and collision detection logic here
```
This is a very basic example to get you started. You'll need to add more functionality, such as obstacle movement, collision detection, and scorekeeping, to create a fully functional game.

Remember, this is just a starting point, and you'll need to learn more about HTML, CSS, and JavaScript to create a more complex game like Spider-Man. Good luck, and have fun!- 
