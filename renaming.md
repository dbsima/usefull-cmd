Recursively rename files with extension .abc to files with extension .xyz

``shell
find  path/to/dir/ -name "*.abc" -exec sh -c 'mv "$1" "${1%.abc}.xyz"' _ {} \;
``

Recursively replace string in all the files of an directory

``shell
grep -rl "/css/" wagtail/wagtail | xargs sed -i s@/css/@/scss/@g
``
