project(
  'tinycthread',
  'c',
  license: 'zlib',
  default_options: [
    'c_std=c99',
    'optimization=3',
    'warning_level=3',
  ])

install_headers('src/tinycthread.h')
static_library(
  'tinycthread',
  'src/tinycthread.c',
  pic: true,
  )
