project('i2cdevlib', 'c', 'cpp',
  default_options : [
    'buildtype=minsize',
    'b_lto=true',
    'cpp_rtti=false',
    'cpp_eh_=none',
    'c_std=gnu11',
    'cpp_std=gnu++11',
    'b_staticpic=false',
  ],
)

assert(meson.is_cross_build(), 'Arduino projects can only be built in a cross build environment.')

subdir('Arduino')
