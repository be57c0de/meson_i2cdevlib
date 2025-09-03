i2cdev_inc_dir = [
    '.',
]

i2cdev_lib = static_library('i2cdev_lib',
  include_directories: i2cdev_inc_dir,
  sources: [ 
    'I2Cdev.cpp',
  ],
  dependencies : [
    subproject('arduinocore-avr').get_variable('arduinocore_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_main_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_wire_dep'),
  ],
)

i2cdev_dep = declare_dependency(
  link_with: i2cdev_lib,
  include_directories: i2cdev_inc_dir,
)
