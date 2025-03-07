cmake_minimum_required(VERSION 3.25)

project(
        Template
        VERSION 0.0.1
        LANGUAGES CXX)
set(PROJECT_LICENSE "MIT")
set(PROJECT_FRIENDLY_NAME ${PROJECT_NAME})
set(PROJECT_LONG_NAME "Template CommonLibSSE-NG")
set(PROJECT_DESCRIPTION ${PROJECT_LONG_NAME})
set(PROJECT_COPYRIGHT "Copyright")

list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake")
include(GNUInstallDirs)
include(addpluginsources)
include(pluginconfig)
include(plugintarget)
include(pluginpackage)
include("${PROJECT_SOURCE_DIR}/local.cmake" OPTIONAL)


# find_library(DETOURS_LIBRARY detours REQUIRED)
# target_include_directories(${PROJECT_NAME} PRIVATE ${DETOURS_INCLUDE_DIRS})
# target_link_libraries(${PROJECT_NAME} PRIVATE ${DETOURS_LIBRARY})