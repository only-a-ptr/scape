file(GLOB EditorMedia_FILES "EditorMedia/*")
file(COPY ${EditorMedia_FILES} DESTINATION "${CMAKE_BINARY_DIR}/bin")

if(EXISTS "${OGRE_CONFIG_DIR}/plugins_d.cfg")
    file(COPY "${OGRE_CONFIG_DIR}/plugins_d.cfg" DESTINATION "${CMAKE_BINARY_DIR}/bin")
endif()

if(EXISTS "${OGRE_CONFIG_DIR}/plugins.cfg")    
    file(COPY "${OGRE_CONFIG_DIR}/plugins.cfg" DESTINATION "${CMAKE_BINARY_DIR}/bin")
endif()
