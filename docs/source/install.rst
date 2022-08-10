Installation
============
Using cmake
------------
Installation using cmake is simple, you just have to compile CPPRAW's source and fetch both nlohmann/json and libcpr using FetchContent.
Add this to your CMakeLists.txt:

.. literalinclude:: cmake.txt
    :linenos:

Manual installation
-------------------
You can probably manually install both `libcpr`_ and `nlohmann/json`_, but preferrably use FetchContent.

_libcpr: https://github.com/libcpr/cpr
_nlohmann/json: https://github.com/nlohmann/json