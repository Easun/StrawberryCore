#
# Copyright (C) 2008-2011 Trinity <http://www.trinitycore.org/>
#
# Copyright (C) 2010-2011 Strawberry Project <http://www.strawberry-pr0jcts.com/>
#
# This file is free software; as a special exception the author gives
# unlimited permission to copy and/or distribute it, with or without
# modifications, as long as this notice is preserved.
#
# This program is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY, to the extent permitted by law; without even the
# implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

if(CMAKE_COMPILER_IS_GNUCXX)
  add_definitions(-fno-delete-null-pointer-checks)
endif()

set(sources_Debugging
  ${CMAKE_SOURCE_DIR}/src/server/shared/Debugging/WheatyExceptionReport.cpp
  ${CMAKE_SOURCE_DIR}/src/server/shared/Debugging/WheatyExceptionReport.h
)
add_subdirectory(shared)
add_subdirectory(game)
add_subdirectory(logonserver)
add_subdirectory(scripts)
add_subdirectory(worldserver)