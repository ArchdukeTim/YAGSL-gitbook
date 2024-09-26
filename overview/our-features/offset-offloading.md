---
description: Store encoder offsets on the motor controller directly
---

# Offset Offloading

{% hint style="danger" %}
This feature is only supported for Spark Max motor controllers
{% endhint %}

Offset Offloading stores the azimuth encoder offset on the motor controller, rather than the roboRIO

To enable offset offloading, use the [`SwerveDrive#pushOffsetsToEncoders`](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#pushOffsetsToEncoders\(\)) method. You can restore roboRIO offset with the [`SwerveDrive#restoreInternalOffset`](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#restoreInternalOffset\(\)) method.
