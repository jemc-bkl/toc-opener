#######################################
# OpENer ports			              #
#######################################

add_subdirectory( ${OpENer_PLATFORM} )

#######################################
# Add common includes                 #
#######################################
opener_common_includes()

#######################################
# Add platform-specific includes      #
#######################################
opener_platform_support("INCLUDES")

set( PLATFORM_GENERIC_SRC generic_networkhandler.c)

add_library( PLATFORM_GENERIC ${PLATFORM_GENERIC_SRC})
