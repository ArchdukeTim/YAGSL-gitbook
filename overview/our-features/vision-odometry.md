---
description: >-
  With the addition of April Tags to the playing field, providing your robot
  with vision can be a huge benefit in having accurate position data.
---

# Vision Odometry

## Combining vision measurements with odometry readings

The [`SwerveDrive` ](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html)class provides an [`addVisionMeasurement` ](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#addVisionMeasurement\(edu.wpi.first.math.geometry.Pose2d,double\))method that allows you to add a reading as well as the timestamp of the reading. This data is usually available from your vision library.

<pre class="language-java" data-full-width="false"><code class="lang-java"><strong>// Readings are retrieved from vision library, such as Limelight or PhotonVision
</strong><strong>Pose2d visionEstimatedPose = ...
</strong><strong>Long visionTimestamp = ...
</strong><strong>swerveDrive.addVisionMeasurement(visionEstimatedPose, visionTimestamp);
</strong></code></pre>
