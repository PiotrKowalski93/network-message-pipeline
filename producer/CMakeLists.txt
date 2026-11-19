add_executable(producer
    main.cpp
    market_data_generator.cpp
    udp_publisher.cpp
)

target_link_libraries(producer
    PRIVATE
        # common
        # Threads::Threads
)