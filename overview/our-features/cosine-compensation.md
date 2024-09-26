---
description: Scale drive vector with the error in azimuth
---

# Cosine Scaling

Any time your swerve module needs to adjust its heading, the robot will briefly move in the wrong direction as the wheels adjust. You can compensate for this by scaling the drive velocity by the error in wheel heading. When the azimuth error is 90 degrees from its target angle, the drive vector will be 0. When the azimuth error is 0 degrees, or at its target angle, the drive vector will be equal to the requested speed.

Enable cosine compensation with the [`SwerveDrive#setCosineCompensator`](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#setCosineCompensator\(boolean\)) method.
