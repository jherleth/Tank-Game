Tank Battle ⚔️🚀

A two-player tank combat game built for the MSPM0G3507 microcontroller with dual ST7735 LCD displays. Players control tanks, adjust their aim with a SlidePot, and fire projectiles with physics-based trajectories. The game combines real-time graphics, input handling, and collision detection in an embedded environment.

Features

🎮 Two-player gameplay – Each player has their own LCD screen to control and battle.
🕹️ SlidePot aiming – Adjust turret angle with an analog input.
💥 Projectile physics – Bullets follow realistic trajectories using integer math optimizations.
📟 Custom graphics engine – Line drawing with Bresenham’s algorithm for efficient rendering.
🔊 Sound effects – Integrated DAC + SysTick for audio feedback.
🧩 Embedded C & ARM assembly – Low-level optimization for performance on MSPM0.

Hardware Used
TI MSPM0G3507 LaunchPad
2 × ST7735R 1.8” TFT LCDs
2 × SlidePots (for aiming control)
Piezo speaker (for sound output)

How It Works
Each player controls their tank on their own screen.
Rotate turret using the SlidePot input.
Press fire button → projectile is simulated and drawn on the screen.
Collision detection determines if a tank is hit.
Game continues until one player wins.

Technical Highlights
Real-time interrupts for input polling, sound playback, and frame updates.
Bresenham’s Line Algorithm for efficient bullet drawing.
FSM (Finite State Machine) manages game states (setup, aiming, firing, collision, win screen).
Memory optimization for running graphics + sound within limited RAM/Flash.

Future Improvements
Power-ups (shield, rapid fire, terrain obstacles)
AI opponent mode
Wireless multiplayer (UART/SPI communication between boards)
Authors

Developed by Jackson Herleth and Adiv Padgilwar
