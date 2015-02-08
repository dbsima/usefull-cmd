Recursively rename files with extension .abc to files with extension .xyz

``shell
find  path/to/dir/ -name "*.abc" -exec sh -c 'mv "$1" "${1%.abc}.xyz"' _ {} \;
``
