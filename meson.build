project('abc', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])

graphene_dep = dependency ('not-found', fallback: ['graphene', 'graphene_dep'])
exe = executable('abc', 'abc.c',
  install : true,
  dependencies: graphene_dep,
  c_args: ['-Werror=double-promotion'])

test('basic', exe)
