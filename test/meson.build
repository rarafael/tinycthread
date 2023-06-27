hello_t = executable('hello', 'hello.c', include_directories: '../src', link_with: static_tinycthread)
test_t = executable('all_test', 'test.c', include_directories: '../src', link_with: static_tinycthread)

test('compiles', hello_t)
test('all', test_t)
