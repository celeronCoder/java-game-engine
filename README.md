# java-game-engine
Game Engine in Java.

# fade-to-black
- It's a desgined test for keyListner utility class.
- Fades the background to black when *space bar* is pressed.

```java
// initialize uitl vars
private float r, g, b, a;
private boolean fadeToBlack = false;

// sets the colour of the initial window to white
private Window() {
	this.width = 1920;
	this.height = 1080;
	this.title = "Jada";

	r = 1;
	g = 1;
	b = 1;
	a = 1;
}

glClearColor(r, g, b, a);

if (fadeToBlack) {
	r = Math.max(r - 0.01f, 0);
	g = Math.max(g - 0.01f, 0);
	b = Math.max(b - 0.01f, 0);
	a = Math.max(a - 0.01f, 0);
}

if (KeyListener.isKeyPressed(GLFW_KEY_SPACE)) {
	fadeToBlack = true;
}
```

#### Note - No Refrence to the game-engine only for testing purpose and fun.