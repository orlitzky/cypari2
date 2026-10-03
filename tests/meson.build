extension_data = {
  'test': files('test.pyx'),
}

foreach name, pyx : extension_data
  py.extension_module(
    name,
    sources: pyx,
    subdir: 'cypari2',
    install: true,
    dependencies: [pari],
    c_args: cysignals_cflags,
    cython_args: cysignals_cythonflags,
    include_directories: [inc_root, include_directories('./../cypari2')],
  )
endforeach

