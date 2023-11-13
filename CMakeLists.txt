cmake_minimum_required(VERSION 3.0.2)
project(cpr_indoornav_ridgeback)

find_package(catkin REQUIRED)

catkin_package(
)

include_directories(
)

install(PROGRAMS
  scripts/environment
  scripts/install
  scripts/ridgeback_power_monitor
  scripts/ridgeback_safety_stop
  scripts/start_ridgeback_bridge

  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

install(DIRECTORY config img launch urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
