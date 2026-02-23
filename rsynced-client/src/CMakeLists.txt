add_executable(rsynced-client)

target_sources(rsynced-client PRIVATE
    main.cpp
)

target_compile_features(rsynced-client PRIVATE cxx_std_23)

target_include_directories(rsynced-client
    PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}
)