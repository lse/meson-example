src = [
  'example.c',
  'thread.c',
  'thread.h',
]

thread_dep = dependency('threads')
curl_dep = dependency('libcurl')
openssl = dependency('openssl')

deps = [
  thread_dep,
  curl_dep,
  openssl,
]

example = executable('example', src, dependencies: deps,
                     include_directories: configuration_inc,
)
