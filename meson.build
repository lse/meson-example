project('example', ['c'], version : '1.0',
  default_options: [
    'c_std=c99',
    'warning_level=2',
  ],
)

conf = configuration_data()
conf.set_quoted('VERSION', '1.0')
conf.set('HAVE_PTHREAD_PRIO_INHERIT', 1)
configure_file(output : 'config.h',
               configuration : conf)
configuration_inc = include_directories('.')

subdir('src')
subdir('tests')
