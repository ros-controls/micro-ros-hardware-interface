# micro-ros-hardware-interface

A micro-ROS-based `ros2_control` hardware interface enables seamless integration of microcontroller-based actuators and sensors with the ROS2 ecosystem by implementing the `hardware_interface::SystemInterface` or `hardware_interface::ActuatorInterface` classes that communicate with embedded devices running micro-ROS agents.

This architecture allows real-time control loops to execute on resource-constrained microcontrollers while exposing standard `ros2_control` command and state interfaces to higher-level controllers. The hardware interface acts as a bridge, translating `ros2_control`'s `read()` and `write()` methods into micro-ROS messages that are sent to/from the microcontroller, enabling distributed control systems where time-critical operations run locally on embedded hardware while benefiting from ROS2's rich ecosystem of planning, perception, and monitoring tools.
