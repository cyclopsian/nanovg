project('nanovg', 'c', license: 'zlib')

cc = meson.get_compiler('c')

add_project_arguments(cc.get_supported_arguments([
  '-Wno-misleading-indentation'
]), language: 'c')

nanovg_inc = include_directories('src')
nanovg_lib = library('nanovg', 'src/nanovg.c')
nanovg = declare_dependency(
  include_directories: nanovg_inc,
  link_with: nanovg_lib
)
