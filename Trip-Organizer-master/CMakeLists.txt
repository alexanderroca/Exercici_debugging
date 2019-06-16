cmake_minimum_required(VERSION 3.13)
project(Trip_Organizer_master)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)
include_directories(data)
include_directories(logic)
include_directories(logic/functions)
include_directories(logic/menu)
include_directories(logic/utils)
include_directories(model)
include_directories(model/destination)
include_directories(model/list)

add_executable(Trip_Organizer_master
        data/mainDatabase.nymal
        data/secondDatabase.nymal
        logic/functions/functions.c
        logic/functions/functions.h
        logic/menu/menu.c
        logic/menu/menu.h
        logic/utils/utils.c
        logic/utils/utils.h
        model/destination/destination.c
        model/destination/destination.h
        model/list/list.c
        model/list/list.h
        main.c
        makefile)
