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
## Table of Contents

- 1. Mobility Management
- Mechanical Design and Steering
- Drivetrain and Weight Distribution
- 2. Sensor Placement Strategy
- 3. Software Architecture
- Control Logic
- 4. Engineering Decisions and Trade-offs
- 5. Performance Limitations and Future Work

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
## Performance Limitations and Future Work☻

While our robot can now complete laps without hitting the outer walls, we are still refining the following areas:
- 1. Speed Consistency: Resolving the intermittent slowdown in the drive motor.
- 2. Obstacle Precision: Improving the "Logic Branches" so the robot can dodge blocks without losing its lane position.
- 3. Parking Execution: Finalizing the timing for the reverse-parking maneuver.
Our team remains focused on these challenges, using each failed test as a way to refine our mechanical and software design.
