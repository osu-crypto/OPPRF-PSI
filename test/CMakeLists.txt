add_executable(psi_analytics_eurocrypt19_test
        psi_analytics_eurocrypt19_test.cpp
        )

target_link_libraries(psi_analytics_eurocrypt19_test PUBLIC
        psi_analytics_eurocrypt19
        gtest
        )

target_include_directories(psi_analytics_eurocrypt19_test PRIVATE
        "${PSI_ANALYTICS_SOURCE_ROOT}/extern/googletest/googletest/include"
        )
        
set_target_properties(psi_analytics_eurocrypt19_test
        PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin"
        )
