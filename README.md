Same code as https://github.com/ros-teleop/teleop_twist_keyboard, changed keybindings

## Usage

```bash
ros2 run tue_teleop_keyboard teleop_twist_keyboard --ros-args -r cmd_vel:=/hero/base/references
```

Parameters: `speed` (0.25), `turn` (0.5), `repeat_rate` (0.0, Hz; 0 publishes only on key press) and
`key_timeout` (0.0, s; 0 waits forever), e.g. `-p speed:=0.5`.

The ROS 1 version lives on the `ros1` branch.
