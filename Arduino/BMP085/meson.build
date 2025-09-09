bmp085_inc_dir = [
    '.',
]

bmp085_lib = static_library('bmp085_lib',
  include_directories: bmp085_inc_dir,
  sources: [ 
    'BMP085.cpp',
  ],
  dependencies : [
    subproject('arduinocore-avr').get_variable('arduinocore_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_main_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_wire_dep'),
    i2cdev_dep,
  ],
)

bmp085_dep = declare_dependency(
  link_with: bmp085_lib,
  include_directories: bmp085_inc_dir,
)
