cmake_minimum_required(VERSION 3.8)
project(tue_teleop_keyboard)

find_package(ament_cmake REQUIRED)

install(
  PROGRAMS src/teleop_twist_keyboard.py
  DESTINATION lib/${PROJECT_NAME}
  RENAME teleop_twist_keyboard
)

if(BUILD_TESTING)
  find_package(ament_cmake_lint_cmake REQUIRED)
  find_package(ament_cmake_xmllint REQUIRED)
  ament_lint_cmake(MAX_LINE_LENGTH 120)
  ament_xmllint(MAX_LINE_LENGTH 120)
endif()

ament_package()
