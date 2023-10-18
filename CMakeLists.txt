add_library(Adafruit_ZeroFFT)

target_link_libraries(Adafruit_ZeroFFT pico_base)
target_include_directories(Adafruit_ZeroFFT PUBLIC ${CMAKE_CURRENT_LIST_DIR}/include)

target_sources(Adafruit_ZeroFFT PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}/fftutil.c 
        ${CMAKE_CURRENT_LIST_DIR}/fftwindows.c
        ${CMAKE_CURRENT_LIST_DIR}/arm_common_tables.c
        )
