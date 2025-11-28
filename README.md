– Smart Automated Bin

Binova is an assistive automated bin designed to make waste disposal more efficient and interactive.
It automatically opens using servo motors, detects objects with an ESP32-CAM, displays messages on an OLED screen, and uses LEDs to indicate system status.
Project Overview
The goal of this project was to design, build, and program a smart bin that could assist users in disposing of waste easily and hands-free.
Although originally planned as a waste sorter, Binova evolved into a fully functional automated smart bin with a clean design, clear feedback indicators, and smooth servo-driven operation.

Components Used
Component	Quantity	Description
ESP32 Development Board	1	Main controller for system operation
ESP32-CAM	1	Captures and classifies objects via Edge Impulse
Servo Motors	3	Controls bin lid movement
OLED Display	1	Displays system status messages
LEDs (Red & Green)	2	Indicates system activity
Breadboard & Jumper Wires	—	For circuit connections
Li-ion Battery Pack	1	Power source
System Workflow
Initialization:
LEDs indicate the system startup sequence.

Detection:
ESP32-CAM captures an image and sends it to the model trained on Edge Impulse.

Classification:
The trained model identifies the object type (e.g., plastic, paper, box).

Action:
The microcontroller commands the appropriate servo motor to open the bin lid.

Feedback:
The OLED screen displays the detected object and LED indicators show operation status.

💻 Software Development
The project integrates:

Edge Impulse for model training and classification accuracy improvement
Arduino IDE for programming both ESP32 and ESP32-CAM
Tinkercad for simulating and testing circuit connections before building
Communication between ESP32 and ESP32-CAM for synchronized control
-pic 38 pic 51

Testing & Troubleshooting
Tested camera accuracy until model reached over 72.5% confidence on Edge Impulse
Debugged servo and OLED control through multiple iterations
Resolved LED indicator errors by re-checking pin mappings
Adjusted power management for stable performance
Screenshot 2025-10-31 114134
Improvements
Enhanced servo alignment for smoother opening/closing
Improved wiring layout for cleaner appearance
Future version will integrate proper waste sorting logic and better camera stabilization
pic 74
Demonstration
A short demo video showcasing Binova in action is available here:
https://youtube.com/shorts/-Wx8wz5JesY?si=5GdPpEyGd8TTJye1

Tools & Platforms
Edge Impulse – for model training
Tinkercad – for circuit design and simulation
Arduino IDE – for programming
GitHub – for version control and documentation
Author
**Mosa Segotlong Created: 2025
Passionate about assistive robotics, automation, and design innovation.

📎 License
This project is shared for educational purposes and can be freely referenced or remixed with proper credit.

About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Releases
No releases published
Create a new release
Packages
No packages published
Publish your first package
Languages
C++
100.0%
Suggested workflows
Based on your tech stack
MSBuild based projects logo
MSBuild based projects
Build a MSBuild based project.
CMake based, single-platform projects logo
CMake based, single-platform projects
Build and test a CMake based project on a single-platform.
SLSA Generic generator logo
SLSA Generic generator
Generate SLSA3 provenance for your existing release workflows
More workflows
Footer

