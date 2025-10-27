env = DefaultEnvironment()

base_path = '#openstack/heat_plugin/'

sources = ['setup.py', 'requirements.txt']
sources += env.AddPythonSources('contrail_heat')
sources += env.AddPythonSources('generated')

sdist_gen = env.Command(
    '/pip/contrail_heat-0.1.dev0-py3-none-any.whl', sources,
    'cd ' + Dir(base_path).path + ' && ' + 'python3 setup.py bdist_wheel --dist-dir /pip')
env.Alias('install', sdist_gen)
