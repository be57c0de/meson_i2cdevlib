mpu6050_inc_dir = [
    '.',
]

mpu6050_lib = static_library('mpu6050_lib',
  include_directories: mpu6050_inc_dir,
  sources: [ 
    'MPU6050_6Axis_MotionApps20.cpp',
    'MPU6050_6Axis_MotionApps612.cpp',
    'MPU6050_9Axis_MotionApps41.cpp',
    'MPU6050.cpp',
  ],
  dependencies : [
    subproject('arduinocore-avr').get_variable('arduinocore_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_main_dep'),
    subproject('arduinocore-avr').get_variable('arduinocore_wire_dep'),
    i2cdev_dep,
  ],
)

mpu6050_dep = declare_dependency(
  link_with: mpu6050_lib,
  include_directories: mpu6050_inc_dir,
)
