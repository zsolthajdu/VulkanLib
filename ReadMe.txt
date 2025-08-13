
# Building on Windows
Requires C++17 or newer, Vulkan SDK, GLFW 3
https://vulkan-tutorial.com/Development_environment#page_Vulkan-Packages

# Linux dependencies
sudo apt install vulkan-tools libvulkan-dev vulkan-validationlayers spirv-tools
sudo apt install libglfw3-dev libglm-dev
Optional : sudo apt install libxxf86vm-dev libxi-dev


# Shaders
To compile shaders use glslc compiler from Vulkan SDK like:

C:\VulkanSDK\1.3.243.0\Bin\glslc.exe shader.vert -o vert.spv
C:\VulkanSDK\1.3.243.0\Bin\glslc.exe shader.frag -o frag.spv
