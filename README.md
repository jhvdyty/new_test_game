new_test_game
A simple interactive OpenGL game prototype written in C++. The goal is to click on a textured square that randomly jumps to a new position upon a successful hit. The game uses GLFW for windowing/input and GLAD for OpenGL function loading.

 Gameplay
You are presented with a colored, textured quad (square) on screen.
Your task is to click on the square with the left mouse button.
Each successful click causes the square to jump to a new random position.

 Features
Basic textured 2D quad rendering

Mouse interaction: hit detection and response

Dynamic quad repositioning using random values

Texture blending with adjustable mix value

Simple keyboard and mouse event handling

 Project Structure
graphql
Копировать код
new_test_game/
├── OpenGL/
│   ├── main.cpp            # Main game logic and rendering
│   ├── shader.h            # Shader loader utility
│   └── stb_image.h         # Image loader for textures
├── texture/
│   ├── brickwall.jpg       # Main texture
│   └── brickwall_normal.jpg# Normal map (blending)
├── vertex.glsl             # Vertex shader
└── fragment.glsl           # Fragment shader
 Controls
Key / Action	Function
W	Increase texture blend factor
S	Decrease texture blend factor
Mouse Left Click	Hit the square to move it randomly
ESC	Exit the game

 Requirements
Make sure you have the following installed:

GLFW (window/input library)

GLAD (OpenGL function loader)

stb_image (texture loader)

OpenGL 3.3 or higher

C++17-compatible compiler

 How to Build
On Linux/macOS
bash
Копировать код
git clone https://github.com/yourusername/new_test_game.git
cd new_test_game

# Install required libraries (example for Debian-based)
sudo apt install libglfw3-dev libglm-dev

# Compile the game
g++ OpenGL/main.cpp -IOpenGL -lglfw -ldl -lGL -o new_test_game
If you're using Windows or another OS, you may need to adapt the compiler and linking commands.

 Running the Game
bash
Копировать код
./new_test_game
📸 Screenshots
![image](https://github.com/user-attachments/assets/be10dbe3-63af-47ae-844b-a0932e2de834)

![image](https://github.com/user-attachments/assets/7148f698-2477-4422-901a-1ab036034bef)

![image](https://github.com/user-attachments/assets/09c18b5d-ee35-48a3-af9f-d8a36ae547fb)


 License
This project is open-source and provided for educational purposes.
Feel free to modify, extend, or use it in your own projects.

