cxx_library(
  name = 'asio',
  header_namespace = 'asio',
  exported_headers = subdir_glob([
    ('asio/include', 'asio.hpp'),
    ('asio/include/asio', '**/*.ipp'),
    ('asio/include/asio', '**/*.hpp'),
  ]),
  srcs = glob([
    'asio/src/asio.cpp',
    'asio/src/asio_ssl.cpp',
  ]),
  preprocessor_flags = [
    '-DASIO_STANDALONE=1',
    '-DASIO_SEPARATE_COMPILATION=1'
  ],
  exported_linker_flags = [
    '-lpthread'
  ],
  visibility = ['PUBLIC']
)
