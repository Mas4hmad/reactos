
add_library(shlwapi_resource_dll MODULE shlwapi_resource_dll.c shlwapi_resource_dll.rc)
set_module_type(shlwapi_resource_dll win32dll ENTRYPOINT DllMain 12)
add_importlibs(shlwapi_resource_dll kernel32 ntdll)
add_dependencies(shlwapi_resource_dll psdk)
