---
description: Orient the wheels when the robot stops moving
---

# Auto-centering Modules

In certain scenarios it may be useful for your swerve modules to reset their positions when there is no input sent from the controllers. One example is when you're at home practicing and wish to make it easier to manually push the robot on the floor. This is only possible if the wheels are oriented the same.

{% hint style="warning" %}
The 'walking' effect caused by gear coupling may cause misalignment of your robot as the modules auto-center.

Auto-centering is not recommended for use during competition.
{% endhint %}

You enable auto-centering by calling [`SwerveDrive#setAutoCenteringModule`](https://broncbotz3481.github.io/YAGSL/swervelib/SwerveDrive.html#setAutoCenteringModules\(boolean\))
