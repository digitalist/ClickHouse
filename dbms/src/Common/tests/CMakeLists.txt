add_executable (hashes_test hashes_test.cpp)
target_link_libraries (hashes_test dbms)

add_executable (sip_hash sip_hash.cpp)
target_link_libraries (sip_hash dbms_common_io)

add_executable (sip_hash_perf sip_hash_perf.cpp)
target_link_libraries (sip_hash_perf dbms_common_io)

add_executable (auto_array auto_array.cpp)
target_link_libraries (auto_array dbms_common_io)

add_executable (lru_cache lru_cache.cpp)
target_link_libraries (lru_cache dbms_common_io)

add_executable (hash_table hash_table.cpp)
target_link_libraries (hash_table dbms_common_io)

add_executable (small_table small_table.cpp)
target_link_libraries (small_table dbms_common_io)

add_executable (parallel_aggregation parallel_aggregation.cpp)
target_link_libraries (parallel_aggregation dbms_common_io)

add_executable (parallel_aggregation2 parallel_aggregation2.cpp)
target_link_libraries (parallel_aggregation2 dbms_common_io)

add_executable (int_hashes_perf int_hashes_perf.cpp AvalancheTest.cpp Random.cpp)
target_link_libraries (int_hashes_perf dbms_common_io)

add_executable (simple_cache simple_cache.cpp)
target_include_directories (simple_cache PRIVATE ${DBMS_INCLUDE_DIR})
target_link_libraries (simple_cache common)

add_executable (compact_array compact_array.cpp)
target_link_libraries (compact_array dbms_common_io ${Boost_FILESYSTEM_LIBRARY})

add_executable (radix_sort radix_sort.cpp)
target_link_libraries (radix_sort dbms_common_io)

add_executable (shell_command_test shell_command_test.cpp)
target_link_libraries (shell_command_test dbms_common_io)

add_executable (arena_with_free_lists arena_with_free_lists.cpp)
target_link_libraries (arena_with_free_lists dbms_common_io)

add_executable (pod_array pod_array.cpp)
target_link_libraries (pod_array dbms_common_io)

add_executable (thread_creation_latency thread_creation_latency.cpp)
target_link_libraries (thread_creation_latency dbms_common_io)

add_executable (thread_pool thread_pool.cpp)
target_link_libraries (thread_pool dbms_common_io)

add_executable (array_cache array_cache.cpp)
target_link_libraries (array_cache dbms_common_io)

add_executable (space_saving space_saving.cpp)
target_link_libraries (space_saving dbms_common_io)

add_executable (integer_hash_tables_and_hashes integer_hash_tables_and_hashes.cpp)
target_include_directories (integer_hash_tables_and_hashes BEFORE PRIVATE ${SPARCEHASH_INCLUDE_DIR})
target_link_libraries (integer_hash_tables_and_hashes dbms_common_io)

add_executable (allocactor allocator.cpp)
target_link_libraries (allocactor dbms)
