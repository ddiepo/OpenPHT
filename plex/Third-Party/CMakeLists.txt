if(ENABLE_TESTING)
  include_directories(gmock gmock/include gtest gtest/include)
  add_library(gmock STATIC gmock/src/gmock-all.cc)
  add_library(gtest STATIC gtest/src/gtest-all.cc gtest/src/gtest_main.cc)
 endif(ENABLE_TESTING)

add_subdirectory(hash-library)
add_subdirectory(aes)