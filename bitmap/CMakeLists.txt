set(HEADERS iff.h)
set(CPPS
  bitmain.cpp
  bumpmap.cpp
  iff.cpp
  lightmap.cpp
  pcx.cpp
  tga.cpp)

add_library(bitmap STATIC ${HEADERS} ${CPPS})
target_link_libraries(bitmap PRIVATE
  cfile
  ddebug
)
