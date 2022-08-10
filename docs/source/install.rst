Installation
============
Using cmake
------------
Installation using cmake is simple, you just have to compile CPPRAW's source and fetch both nlhomann/json and libcpr using FetchContent.
Add this to your CMakeLists.txt:

.. code-block:: cmake
    add_executable(your_proyect main.cpp CPPRAW/*.cpp)

    include(FetchContent)

    FetchContent_Declare(cpr GIT_REPOSITORY https://github.com/libcpr/cpr.git GIT_TAG 871ed52d350214a034f6ef8a3b8f51c5ce1bd400)
    FetchContent_MakeAvailable(cpr)
    FetchContent_Declare(json URL https://github.com/nlohmann/json/releases/download/v3.11.1/json.tar.xz)
    FetchContent_MakeAvailable(json)
    
    target_link_libraries(your_proyect PRIVATE nlohmann_json::nlohmann_json)
    target_link_libraries(your_proyect PRIVATE cpr::cpr)