set(LIEF_PYTHON_PE_SRC
  "${CMAKE_CURRENT_LIST_DIR}/objects/signature/pySignerInfo.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/signature/pyAuthenticatedAttributes.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/signature/pyx509.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/signature/pyContentInfo.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/signature/pySignature.cpp"

  "${CMAKE_CURRENT_LIST_DIR}/objects/pyDataDirectory.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyDosHeader.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyBuilder.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyOptionalHeader.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyRelocationEntry.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyBinary.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyResourcesManager.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyHeader.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyDebug.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pySection.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyExport.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyImport.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyExportEntry.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyRelocation.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyParser.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyImportEntry.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pySymbol.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/objects/pyTLS.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/pyPEStructures.cpp"
  "${CMAKE_CURRENT_LIST_DIR}/pyPE.cpp"
)

target_include_directories(pyLIEF PUBLIC "${CMAKE_CURRENT_LIST_DIR}")
target_sources(pyLIEF PRIVATE "${LIEF_PYTHON_PE_SRC}")



