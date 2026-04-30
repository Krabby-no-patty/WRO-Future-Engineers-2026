# WRO-Future-Engineers-2026
Autonomous self-driving car for WRO Future Engineers 2026

## Group name♥︎
team name:krabby-no-patty
teammates:
- Caleb Jair Rosa Roman
- Angelica Victoria Colon Berrios 
- Reynaldo Gariel Colon Berrios

- country / región:Puerto Rico

---

## Team Introduction★

We are a team of three students from Puerto Rico—two 16-year-olds and one 14-year-old—competing in the WRO Future Engineers category. This repository documents our journey of building and programming an autonomous vehicle using the LEGO SPIKE Prime system.

---

## Mechanical Design and Steering♡

Our initial prototype had a major flaw: the steering range was too narrow. The front wheels would hit the Technic beams before reaching the angle needed for sharp turns. To fix this, we redesigned the front assembly to be more open. By trimming the frame and adjusting the gear linkage, we gained the "turn-headroom" necessary to avoid wall collisions. 

- Drivetrain and Weight Distribution:

The robot uses a Rear-Wheel Drive (RWD) configuration. We placed the LEGO SPIKE Hub and the drive motor in the back to ensure the weight is centered over the traction tires.
- Dimensions: Width: 18.5 cm | Length: 27.5 cm | Height: 9.5 cm.
- Current Challenge: We have observed an occasional slowdown in the drivetrain. We are currently investigating if this is caused by mechanical friction in the rear axle or a power-drop in the hub. 

---

## Sensor Placement Strategy◎

The sensing system is designed for real-time environmental awareness using a triple ultrasonic array.
- Configuration: We use three sensors labeled F (Front), B (Left), and D (Right).
- Reaction Time: The front sensor is mounted at the leading edge of the robot to maximize detection distance. This gives the program more time to stop or turn when an obstacle appears.
- Cable Management: We used a ribbon-routing strategy to secure all wires through the center of the frame. This prevents cables from interfering with the steering motor or snagging on external obstacles during a run.

---

## Software Architecture□

Our robot is programmed using LEGO SPIKE Word Blocks. We chose this environment to allow for fast debugging and visual logic tracking during our limited testing sessions.

---
## Engineering Decisions and Trade-offs☻

The following table highlights the key decisions made to improve system performance:

![Decision Table](images/IMG_6312.png)
