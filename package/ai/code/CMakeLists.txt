cmake_minimum_required(VERSION 3.2)
project(ai C CXX)

#set(DEMO_ROOT "${PROJECT_SOURCE_DIR}/../crb_demo")
set(CMAKE_C_FLAGS_DEBUG "-O0 -g3")
set(CMAKE_C_FLAGS_RELEASE "-O2 -s")
set(CMAKE_CXX_FLAGS_DEBUG "-O0 -g3")
set(CMAKE_CXX_FLAGS_RELEASE "-O2 -s")
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fopenmp")

add_subdirectory(face_detect)
add_subdirectory(face_landmarks)
add_subdirectory(object_detect)
add_subdirectory(face_alignment)
add_subdirectory(face_expression)
add_subdirectory(head_pose_estimation)
add_subdirectory(face_recog)
add_subdirectory(simple_pose)
add_subdirectory(openpose)
add_subdirectory(person_detect)
add_subdirectory(hand_image_classify)
add_subdirectory(license_plate_recog)
add_subdirectory(self_learning)
add_subdirectory(object_detect_demo)
add_subdirectory(retinaface_mb_320)


