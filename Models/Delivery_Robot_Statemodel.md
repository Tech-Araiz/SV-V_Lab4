| ID | State Name | Description | Entry Condition | Exit Condition |
|---|---|---|---|---|
| **S1** | IDLE | The robot is waiting at the warehouse for a delivery request. | System is powered on OR the robot reaches the warehouse after a journey. | A valid delivery request is received. |
| **S2** | NAVIGATING | The robot moves toward the destination while monitoring its path and battery level. | A delivery request is received while IDLE OR an obstacle is cleared during AVOIDING_OBSTACLE. | Destination is reached, an obstacle is detected, OR battery becomes critically low. |
| **S3** | AVOIDING_OBSTACLE | The robot suspends regular navigation to maneuver around a detected obstacle. | An obstacle is detected while NAVIGATING. | Obstacle is successfully avoided and cleared. |
| **S4** | DELIVERING | The robot executes the package handoff process at the destination. | The robot reaches the target destination from NAVIGATING. | Package delivery process is completed successfully. |
| **S5** | RETURNING | The robot navigates back to the warehouse. | Delivery is completed OR battery becomes critically low during NAVIGATING. | The robot reaches the warehouse. |
