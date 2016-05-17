project(vehicle_detection C CXX)
cmake_minimum_required(VERSION 3.2)

find_package(OpenCV 3.1 REQUIRED)


set(SRC
	vehicle_detection.cpp
)

add_executable(VEHICLE ${SRC})
target_link_libraries( VEHICLE
					   ${OpenCV_LIBS}				
)