cmake_minimum_required(VERSION 3.5)
project(flex_bt_turtlebot_demo_flexbe_states)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_python REQUIRED)
find_package(rclcpp REQUIRED)
find_package(rclpy REQUIRED)

INSTALL(DIRECTORY
    launch
    DESTINATION share/${PROJECT_NAME}
)

INSTALL(DIRECTORY
    test
    DESTINATION share/${PROJECT_NAME}
)

# Install Python modules
ament_python_install_package(${PROJECT_NAME})

ament_package()
