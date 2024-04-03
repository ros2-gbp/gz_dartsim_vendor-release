cmake_minimum_required(VERSION 3.10)
project(gz_dartsim_vendor)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_vendor_package REQUIRED)

ament_vendor(${PROJECT_NAME}
  VCS_URL https://github.com/dartsim/dart.git
  VCS_VERSION v6.13.2
  CMAKE_ARGS
    -DDART_BUILD_GUI_OSG:BOOL=FALSE
    -DDART_BUILD_DARTPY:BOOL=FALSE
    -DDART_BUILD_EXTRAS:BOOL=FALSE
  GLOBAL_HOOK
  PATCHES patches
)

if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)
  ament_lint_auto_find_test_dependencies()
endif()

ament_package()
