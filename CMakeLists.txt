cmake_minimum_required(VERSION 3.16)

idf_component_register(SRC_DIRS . u8g2/csrc
                    INCLUDE_DIRS include u8g2/csrc
                    REQUIRES driver freertos)

target_link_directories(${COMPONENT_LIB} PRIVATE u8g2/csrc)
target_link_libraries(${COMPONENT_LIB})
