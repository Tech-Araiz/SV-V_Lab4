| Req. ID | Requirement | Description | Priority |
|---------|-------------|-------------|----------|
| **R1** | The robot shall enter **Idle mode** when switched on and wait for a delivery request. | Sets initial startup state. | **High** |
| **R2** | The robot shall start moving to the destination upon receiving a delivery request while idle. | Triggers delivery journey. | **High** |
| **R3** | The robot shall continuously check surroundings while moving. | Enables obstacle detection. | **High** |
| **R4** | The robot shall stop normal movement and enter **Obstacle-Avoidance mode** when an obstacle is detected. | Prevents collisions. | **High** |
| **R5** | The robot shall resume moving toward the destination once the obstacle is cleared. | Restores target navigation. | **High** |
| **R6** | The robot shall start the delivery process upon reaching the destination. | Handles package handoff. | **High** |
| **R7** | The robot shall start returning to the warehouse after the package is delivered. | Initiates return leg. | **High** |
| **R8** | The robot shall monitor battery level and return to the warehouse if the battery is critically low. | Prevents complete battery drainage. | **High** |
| **R9** | The robot shall re-enter **Idle mode** upon returning to the warehouse. | Prepares for next task. | **High** |
| **R10** | The robot shall not start delivery directly from Idle mode or while in Obstacle-Avoidance mode. | Restricts invalid transitions. | **High** |
