add_executable(ethvm main.cpp)

target_link_libraries(ethvm PRIVATE ethereum evm ethashseal devcore Boost::program_options cryptopp-static)

target_include_directories(ethvm PRIVATE ../utils)

install(TARGETS ethvm DESTINATION bin OPTIONAL)
