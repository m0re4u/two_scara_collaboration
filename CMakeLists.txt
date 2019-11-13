cmake_minimum_required(VERSION 2.8.3)
project(two_scara_collaboration)

find_package(catkin_simple REQUIRED)

catkin_simple()

cs_add_executable(scara_joint_controller src/scara_joint_controller.cpp)
cs_add_executable(scara_left_motion_planner src/scara_left_motion_planner.cpp)

cs_install()
cs_export()
