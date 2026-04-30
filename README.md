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
- Torque/Speed Reasoning:
  We chose a gear ratio that favors torque. We realized that maintaining a consistent speed through corners is more valuable than high top speeds that lead to "drifting" into the walls.

---

## Sensor Placement Strategy◎

- Configuration: We use three sensors labeled F (Front), B (Left), and D (Right).
- Placement Rationale: Side sensors are placed at the widest point of the chassis to get the most accurate "distance-to-wall" readings. The front sensor is mounted low to ensure it detects obstacles before the bumper makes contact.
- Failure-Point Mitigation: We identified that ultrasonic sensors can sometimes provide "ghost readings". Our code is being tuned to cross-reference the B and D sensors; if one gives an impossible value, the robot relies on the other to maintain its lane.
- Wiring and Port Management
- Organization: All ribbon cables are routed through the internal Technic frame.
- Risk Identification: We learned that loose cables can snag on the steering rack. We used secure clips to ensure that the mechanical movement of the steering does not interfere with the electronic signals.

---

## Software Architecture□

Our robot is programmed using LEGO SPIKE Word Blocks. We chose this environment to allow for fast debugging and visual logic tracking during our limited testing sessions.

---
## Performance Metrics and Future Work

We don't just guess; we measure.
- Metric 1: After our steering rebuild, our turning radius decreased by roughly 35%, allowing us to stay 10cm further away from the outer wall during turns.
-  Metric 2: Success rate of obstacle avoidance is currently 60%—we are working to reach 90% by refining our sensor-check frequency.
- Future Work: Our biggest goal is solving the "slowdown" mystery and perfecting our reverse-parking logic for the final challenge.
