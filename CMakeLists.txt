cmake_minimum_required(VERSION 3.1)
project(SofaPython)


# OPTIONS
find_package(PythonLibs 2 QUIET)
option(SOFA_PYTHON_WITH_PYTHON_2 "Compile the plugin with python 2 support" ${PYTHONLIBS_FOUND})

find_package(PythonLibs 3 QUIET)
option(SOFA_PYTHON_WITH_PYTHON_3 "Compile the plugin with python 3 support" ${PYTHONLIBS_FOUND})

if (SOFA_PYTHON_WITH_PYTHON_2)
    message(STATUS " WITH PYTHON 2 SUPPORT (version ${PYTHONLIBS_VERSION_STRING})")
endif()

if (SOFA_PYTHON_WITH_PYTHON_3)
    message(STATUS " WITH PYTHON 3 SUPPORT (version ${PYTHONLIBS_VERSION_STRING})")
endif()