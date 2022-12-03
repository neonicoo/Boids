cmake_minimum_required(VERSION 3.23)
project(boids)

set(CMAKE_CXX_STANDARD 14)
find_package(SFML 2.5.1 COMPONENTS graphics)

include_directories(src)

add_executable(boids
        src/Boid.cpp
        src/Boid.h
        src/Flock.cpp
        src/Flock.h
        src/Game.cpp
        src/Game.h
        src/main.cpp
        src/Pvector.cpp
        src/Pvector.h)

target_link_libraries(boids sfml-graphics)
