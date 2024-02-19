add_executable(vulkan_try
        src/main.cpp
    )

target_link_libraries(vulkan_try PRIVATE ecs)
target_link_libraries(vulkan_try PRIVATE glfw)
target_link_libraries(vulkan_try PRIVATE vulkan)


if(NDEBUG)
    target_compile_definitions(vulkan_try PRIVATE
        NDEBUG)
endif()
