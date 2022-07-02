# CMakeList.txt : CMake project for HelloVulkan, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
# https://heishenhua.com
add_executable (HelloVulkan "HelloVulkan.cpp" )

# Windows library dependencies
include_directories( "C:/Users/z_haj/Documents/Visual Studio 2022/Libraries/glfw-3.3.7/include"
				"C:/Users/z_haj/Documents/Visual Studio 2022/Libraries/glm"
				"C:/VulkanSDK/1.3.216.0/Include"
	)
	
target_link_directories( HelloVulkan PUBLIC  "C:/Users/z_haj/Documents/Visual Studio 2022/Libraries/glfw-3.3.7.bin.WIN64/lib-vc2022"
				"C:/VulkanSDK/1.3.216.0/Lib"
	)


target_link_libraries( HelloVulkan glfw3 vulkan-1  )

# TODO: Add tests and install targets if needed.
