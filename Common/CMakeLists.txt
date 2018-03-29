cmake_minimum_required(VERSION 3.1)
project(SofaPythonCommon)

# Python 2.7 AND Python 3 compatible files
set(HEADER_FILES
        Common.h
        Macros.h
)

set(SOURCE_FILES

)

# Python 2.7 only
if (SOFA_PYTHON_WITH_PYTHON_2)
    find_package(PythonLibs 2 REQUIRED)

endif()


