if(USE_PYTHON)
    add_test(NAME pytest COMMAND ${PYTHON_EXECUTABLE} -m pytest WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})
    add_custom_target(pytest ${PYTHON_EXECUTABLE} -m pytest WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})
    set_tests_properties ( pytest PROPERTIES TIMEOUT 1800 )
endif(USE_PYTHON)
