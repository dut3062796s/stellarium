SET(OBSERVABILITY_VERSION "1.2.4")

SET(CMAKE_INSTALL_PREFIX $HDATALOC)
ADD_DEFINITIONS(-DOBSERVABILITY_PLUGIN_VERSION="${OBSERVABILITY_VERSION}")
ADD_DEFINITIONS(-DOBSERVABILITY_PLUGIN_LICENSE="GNU GPLv2 or later")

ADD_SUBDIRECTORY( src )

INSTALL(FILES DESTINATION "modules/Observability")
