project('dyad', 'c')

dyad_lib = library(
  'dyad',
  sources: files(
    'src/dyad.c',
    # the src/*.c files are not needed
    # they are included (#line 1 "src/foo.c")
  ),
  include_directories: [
    include_directories('src')
  ],
  c_args: [
    ]
)
dyad_dep = declare_dependency(
  link_with: dyad_lib,
  include_directories: include_directories('src'),
)
