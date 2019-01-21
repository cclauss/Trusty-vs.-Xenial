# Trusty-vs.-Xenial
__Q:__ What is the best way to determine the current distro?

__A:__
```python
import platform
uname_version = platform.uname().version
IS_DIST_XENIAL = '-Ubuntu' in uname_version and '16.04' in uname_version
```
## dist: trusty
```
$ python platform_info.py
         architecture() = ('64bit', 'ELF')
                 dist() = ('debian', 'jessie/sid', '')
             libc_ver() = ('glibc', '2.3.4')
   linux_distribution() = ('debian', 'jessie/sid', '')
              machine() = x86_64
                 node() = travis-job-6d2bf4d4-8483-44bf-a3f3-fd1dc72fcaa2
             platform() = Linux-4.4.0-101-generic-x86_64-with-debian-jessie-sid
            processor() = x86_64
         python_build() = ('default', 'Nov 28 2017 18:47:21')
      python_compiler() = GCC 4.8.4
python_implementation() = CPython
       python_version() = 3.6.3
 python_version_tuple() = ('3', '6', '3')
              release() = 4.4.0-101-generic
               system() = Linux
                uname() = uname_result(system='Linux', node='travis-job-6d2bf4d4-8483-44bf-a3f3-fd1dc72fcaa2', release='4.4.0-101-generic', version='#124~14.04.1-Ubuntu SMP Fri Nov 10 19:05:36 UTC 2017', machine='x86_64', processor='x86_64')
              version() = #124~14.04.1-Ubuntu SMP Fri Nov 10 19:05:36 UTC 2017
linux 3.6.3 (default, Nov 28 2017, 18:47:21) 
[GCC 4.8.4]
```
## dist: xenial
```
$ python platform_info.py
         architecture() = ('64bit', 'ELF')
                 dist() = ('debian', 'stretch/sid', '')
             libc_ver() = ('glibc', '2.3.4')
   linux_distribution() = ('debian', 'stretch/sid', '')
              machine() = x86_64
                 node() = travis-job-9404cf56-53dd-47b3-9596-6a9f82a89cfe
             platform() = Linux-4.15.0-1026-gcp-x86_64-with-debian-stretch-sid
            processor() = x86_64
         python_build() = ('default', 'Nov 28 2018 13:38:24')
      python_compiler() = GCC 5.4.0 20160609
python_implementation() = CPython
       python_version() = 3.6.7
 python_version_tuple() = ('3', '6', '7')
              release() = 4.15.0-1026-gcp
               system() = Linux
                uname() = uname_result(system='Linux', node='travis-job-9404cf56-53dd-47b3-9596-6a9f82a89cfe', release='4.15.0-1026-gcp', version='#27~16.04.1-Ubuntu SMP Fri Dec 7 09:59:47 UTC 2018', machine='x86_64', processor='x86_64')
              version() = #27~16.04.1-Ubuntu SMP Fri Dec 7 09:59:47 UTC 2018
linux 3.6.7 (default, Nov 28 2018, 13:38:24) 
[GCC 5.4.0 20160609]
```
