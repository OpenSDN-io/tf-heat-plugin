# -*- mode: python; -*-

env = DefaultEnvironment()

base_path = '#openstack/heat_plugin/'

sdist_gen = env.Command(
    '/pip/contrail_heat-0.1.dev0-py3-none-any.whl', 'setup.py',
    'cd ' + Dir(base_path).path + ' && ' + 'python3 setup.py bdist_wheel --dist-dir /pip')
env.Alias('install', sdist_gen)
