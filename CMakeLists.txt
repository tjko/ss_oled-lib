add_library(ss_oled-lib INTERFACE)
target_include_directories(ss_oled-lib INTERFACE ${CMAKE_CURRENT_LIST_DIR})
target_link_libraries(ss_oled-lib INTERFACE hardware_i2c)
target_sources(ss_oled-lib INTERFACE
  ${CMAKE_CURRENT_LIST_DIR}/ss_oled.h
  ${CMAKE_CURRENT_LIST_DIR}/ss_oled.c
  ${CMAKE_CURRENT_LIST_DIR}/BitBang_I2C.h
  ${CMAKE_CURRENT_LIST_DIR}/BitBang_I2C.c
)
