# CMakeList.txt : CMake project for HelloVulkan, include source and define
# project specific logic here.
#
# REQUIRES C++x17 minimum

cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
# https://heishenhua.com
add_executable (HelloVulkan "HelloVulkan.cpp" )

include_directories(${PROJECT_SOURCE_DIR}/include)

# Windows library dependencies
include_directories( "C:/Users/z_haj/Devel/Libraries/glfw-3.3.8/include"
				"C:/Users/z_haj/Devel/Libraries/glm"
				"C:/VulkanSDK/1.3.243.0/Include"
	)
	
target_link_directories( HelloVulkan PUBLIC  "C:/Users/z_haj/Devel/Libraries/glfw-3.3.8.bin.WIN64/lib-vc2019"
				"C:/VulkanSDK/1.3.243.0/Lib"
	)


target_link_libraries( HelloVulkan glfw3 vulkan-1  )

# TODO: Add tests and install targets if needed.
