# CMakeList.txt : CMake project for CMakeProject1_delete, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (CMakeProject1_delete "CMakeProject1_delete.cpp" "CMakeProject1_delete.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CMakeProject1_delete PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
add_custom_target(testTarget COMMAND "ls" "-al")