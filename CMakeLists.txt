cmake_minimum_required(VERSION 3.8)
project(pool_simulator)

find_package(ament_cmake REQUIRE)

install(DIRECTORY launch models world DESTINATION share/${PROJECT_NAME})
ament_package()