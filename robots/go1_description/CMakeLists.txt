cmake_minimum_required(VERSION 2.8.3)
project(go1_description)

find_package(catkin REQUIRED COMPONENTS
    genmsg
    roscpp
    std_msgs
    tf
    wx250_description
)

catkin_package(
    CATKIN_DEPENDS roscpp std_msgs wx250_description # Add wx250_description here
)

include_directories(
    ${Boost_INCLUDE_DIR}
    ${catkin_INCLUDE_DIRS}
)
