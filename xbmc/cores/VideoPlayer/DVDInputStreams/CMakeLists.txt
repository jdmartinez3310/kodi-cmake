set(SOURCES DVDFactoryInputStream.cpp
            DVDInputStream.cpp
            DVDInputStreamFFmpeg.cpp
            DVDInputStreamFile.cpp
            DVDInputStreamMemory.cpp
            DVDInputStreamMpegDash.cpp
            DVDInputStreamNavigator.cpp
            DVDInputStreamPVRManager.cpp
            DVDInputStreamRTMP.cpp
            DVDInputStreamStack.cpp
            DVDStateSerializer.cpp)


if(BLURAY_FOUND)
  list(APPEND SOURCES DVDInputStreamBluray.cpp)
endif()

core_add_library(dvdinputstreams)
add_dependencies(dvdinputstreams libcpluff dvdnav ffmpeg)
