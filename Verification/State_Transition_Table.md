| ID | From State | Event / Condition | To State | Action / Requirement |
|---|---|---|---|---|
| **T1** | IDLE | Delivery request received | NAVIGATING | Initialize destination coordinates and start movement toward target destination. |
| **T2** | NAVIGATING | Obstacle in proximity detected | AVOIDING_OBSTACLE | Pause standard pathing and engage localized evasion maneuver. |
| **T3** | AVOIDING_OBSTACLE | Path cleared & obstacle passed | NAVIGATING | Recalculate trajectory and resume forward transit to destination. |
| **T4** | NAVIGATING | Target coordinates reached | DELIVERING | Halt drivetrain and trigger package release mechanism. |
| **T5** | DELIVERING | Handshake/delivery confirmation received | RETURNING | Secure compartment and plot return vector back to warehouse. |
| **T6** | RETURNING | Home base / warehouse reached | IDLE | Power down transit systems and await next assignment queue. |
| **T7** | NAVIGATING | Battery level <= critical threshold | RETURNING | Abort mission parameters and reroute directly to warehouse charging point. |
