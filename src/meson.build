inc = include_directories('.', '../..', '../')

dep_e = dependency('enlightenment')
deps = [
        dep_e,
        dependency('elementary')
]

src = [
  'tageslosung.h',
  'main.c',
  'config.c'
]

executable('tageslosung',
  src,
  dependencies: deps,
  c_args : ['-fPIE', '-fPIC'],
  link_args : ['-rdynamic', '-pie'],
  install_dir: install_dir,
  install: true,
  include_directories: inc
)
