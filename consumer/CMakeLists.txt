add_executable(consumer
    main.cpp
)

target_link_libraries(consumer
    PRIVATE
        # common
        # Threads::Threads
)