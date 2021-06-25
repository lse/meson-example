check_output = find_program('test-args')

test('Dummy test in C',
     executable('test-example', 'test-example.c', dependencies: deps)
)
test('Test in shell', check_output,  depends: example)
