project(MyTests)

include(${CMAKE_SOURCE_DIR}/cmake/UnitTests.cmake)

add_boost_test(btest01 btest01.cpp)
target_link_libraries(btest01 MyMath)

add_gmock_test(gtest01 gtest01.cpp)
target_link_libraries(gtest01 MyMath)
