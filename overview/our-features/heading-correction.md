---
description: Automatically maintain robot orientation while driving across the field
---

# Heading Correction

Heading correction is used to keep the robot heading the same as the previous heading while the robot is translating. It is aggressive and will prevent angular rotation based control schemes from working.

## Configuration

#### Enable / Disable

Heading correction can be enabled via  the [`SwerveDrive#setHeadingCorrection`](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#setHeadingCorrection\(boolean,double\)) method.

#### Deadband

Heading correction only enables when the requested rotation speed is **below** a certain threshold, and the requested translation speed is **above** a certain threshold. By default the deadband is `.01 rad / s` and `.01 m / s` respectively. You can set a custom deadband as a second argument to the `setHeadingCorrection` method.

{% hint style="info" %}
A single deadband value is used for both rotation and translation
{% endhint %}

