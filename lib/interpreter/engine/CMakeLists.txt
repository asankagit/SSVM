# SPDX-License-Identifier: Apache-2.0

add_library(ssvmInterpreterEngine
  control.cpp
  table.cpp
  memory.cpp
  variable.cpp
  engine.cpp
)

target_link_libraries(ssvmInterpreterEngine
  PRIVATE
  ssvmCommon
)

target_include_directories(ssvmInterpreterEngine
  PUBLIC
  ${Boost_INCLUDE_DIR}
  ${PROJECT_SOURCE_DIR}/include
  ${PROJECT_SOURCE_DIR}/thirdparty
)
