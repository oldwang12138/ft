
add_library(base STATIC
    contract_table.cpp)
add_library(ft::base ALIAS base)

target_include_directories(base PRIVATE "${PROJECT_SOURCE_DIR}/src")
target_link_libraries(base PUBLIC ft::ft_header ft::ft_third_party)
