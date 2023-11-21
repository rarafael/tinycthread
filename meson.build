project(
  'tinycthread',
  'c',
  license: 'zlib',
  license_files: 'LICENSE',
  version: '1.2',
  default_options: [
    'c_std=c99',
    'optimization=3',
    'warning_level=3',
  ])

install_headers('src/tinycthread.h')
static_tinycthread = static_library(
  'tinycthread',
  'src/tinycthread.c',
  pic: true,
  install: true,
  )
pkg = import('pkgconfig')
pkg.generate(
  static_tinycthread,
  description: 'Basic threading classes for C',
  filebase: 'tinycthread',
  name: 'tinycthread',
  )

tinycthread_dep = declare_dependency(
  link_with: static_tinycthread,
  include_directories: './src/')

subdir('test')
