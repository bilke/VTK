IF(NOT VTK_INSTALL_NO_RUNTIME)

  CONFIGURE_FILE(
    ${CMAKE_CURRENT_SOURCE_DIR}/vtktextanalysis.tcl.in
    ${CMAKE_CURRENT_BINARY_DIR}/vtktextanalysis.tcl
    @ONLY)

  INSTALL(FILES
    ${CMAKE_CURRENT_BINARY_DIR}/vtktextanalysis.tcl
    DESTINATION ${VTK_TCL_INSTALL_DIR_CM24}/vtktextanalysis
    COMPONENT RuntimeLibraries)
ENDIF(NOT VTK_INSTALL_NO_RUNTIME)
