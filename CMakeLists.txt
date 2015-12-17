cmake_minimum_required(VERSION 2.8)
project(nba_impact_stats)

find_package(CURL)

add_executable(json_reader src/nba_json.cpp)
target_link_libraries(json_reader ${CURL_LIBRARIES})
